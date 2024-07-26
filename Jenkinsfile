pipeline {
    agent any
    environment {
        DEPLOY_TO = 'prod'
    }
    parameters {
        sring(name: 'TEST' , defaultValue:'Tests unitaires' , description:'test description')
    }
    stages {
        stage ('build') {
            steps {
              echo "Build !!"
            }
        }
        stage ('deployment production') {
            allOf {
                environment name: 'DEPLOY_TO' , value: 'prod'
                equals expected : 'Tests unitaires' , actual : params.TEST
            }
            steps {
                echo "Deploy !!!"
            }
}
    }
}
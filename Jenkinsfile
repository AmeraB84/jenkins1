pipeline {
    agent any
    environment {
        DEPLOY_TO : false
    }
    stages {
        stage ('build') {
            steps {
              echo "Build !!"
            }
        }
        stage ('deployment production') {
            when {
                environment name: 'DEPLY_TO' , value: true
            }
            steps {
                echo "${VERSION} Deployed by ${USER}"
            }
}
    }
}
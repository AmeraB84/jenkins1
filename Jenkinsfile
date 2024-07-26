pipeline {
    agent any
    environment {
        DEPLOY_TO = true
    }
    stages {
        stage ('build') {
            steps {
              echo "Build !!"
            }
        }
        stage ('deployment production') {
            when {
                environment name: 'DEPLOY_TO' , value: 'true'
            }
            steps {
                echo "${VERSION} Deployed by ${USER}"
            }
}
    }
}
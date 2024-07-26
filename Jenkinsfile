pipeline {
    agent any
    environment {
        DEPLOY_TO = 'prod'
    }
    stages {
        stage ('build') {
            steps {
              echo "Build !!"
            }
        }
        stage ('deployment production') {
            when {
                environment name:DEPLOY_TO, value: 'prod'
            }
            steps {
                echo "${VERSION} Deployed by ${USER}"
            }
}
    }
}
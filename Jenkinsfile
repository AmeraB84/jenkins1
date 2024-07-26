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
                expression { env.DEPLOY_TO == 'prod' }
            }
            steps {
                echo "${VERSION} Deployed by ${USER}"
            }
}
    }
}
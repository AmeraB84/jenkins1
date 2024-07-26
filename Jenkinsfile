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
                expression { env.DEPLOY_TO == true }
            }
            steps {
                echo "${VERSION} Deployed by ${USER}"
            }
}
    }
}
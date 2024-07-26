pipeline {
    agent any

    stages {
        stage ('build') {
            steps {
              echo "Build !!"
            }
        }
        stage ('deployment production') {
            input {
                message 'Would you deploy this version ?'
                ok 'Deployer !'
                submitter 'admin,devops'
                submitterParameter 'USER'
                parameters {
                    string(name:'VERSION',defaultValue:'version1',description:'une version')
                }
            }
            steps {
                echo "${VERSION} Deployed by ${USER}"
            }
}
    }
}
pipeline {
    agent any
    parameters {
        text(name:'PERSONNE',defaultValue:'Mme BOUDIA',description:'Hello amera')
        choice(name:'CHOIX',choices:['un','deux','trois'])
    }
    stages {
        stage ('build') {
            steps {
              echo "la personne est : ${PERSONNE}"
              echo "Son choix est : ${CHOIX}"
            }
        }
    }
}
  
pipeline {
    agent any
    parameters {
        choice(choices: ['bs003' , 'bs0011', 'bs0013', 'bs0014', 'dellshare'], description: 'Select Environment', name: 'Portal')
    }
    stages {
    stage("AUTH") {
        steps { dir("infra") { sh "echo ${params.Portal}" } }
    }
    }

}

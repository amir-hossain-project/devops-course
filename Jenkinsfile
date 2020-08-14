  
pipeline {
    agent any
    parameters {
        choice(choices: ['bs003' , 'bs0011', 'bs0013', 'bs0014', 'dellshare'], description: 'Select Portal', name: 'Portal')
    }
    stages {
    stage("Deploy") {
        steps { dir("Package") { sh "echo ${params.Portal}" } }
    }
    }

}

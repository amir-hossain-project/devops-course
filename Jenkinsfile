pipeline {
  agent any
  stages {
    stage('Check env') {
      steps {
        script {
          if ( env.Environment.isEmpty() ) {
            echo "Environment not specified."
            autoCancelled = true
            error('Aborting the build.')
          }
          else {
            echo "Environment total: ${env.Environment}"
            String[] Env_Array = "${params.Environment}".split(',');
            for (x in Env_Array) {
              echo "ENV: ${x}"
            }
          }
        }
      }
    }
  }
}

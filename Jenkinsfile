pipeline {
   agent none
   environment {
       color = 'blue'
      BUILD_DISPLAY_NAME='Anand Jain'
   }
   stages {
       stage('example') {
            agent { label 'master' }
            steps {
               script {
                  env.BUILD_DISPLAY_NAME='Anand'
               }
            }
        }
    }
}

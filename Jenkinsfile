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
                   def fields = env.getEnvironment()
                   fields.each {
                        key, value -> println("${key} = ${value}");
                    }
 
                    println(env.PATH)
               }
            }
        }
    }
}

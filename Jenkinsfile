pipeline {
    agent any
    environment {
        APP_WAR_NAME = "crewpro#autodial"
    }
    stages {
        stage("Build"){
            steps {
                script {
                    currentBuild.displayName = "${APP_WAR_NAME}"
                    currentBuild.description = "The best description."
                }
            }
        }
    }
}

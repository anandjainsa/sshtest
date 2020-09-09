pipeline {
    agent any
    environment {
        ENV = "crewpro#autodial"
    }
    stages {
        stage("Build"){
            steps {
                script {
                    currentBuild.displayName = "${ENV}-${env.BRANCH_NAME}-${currentBuild.id}"
                    currentBuild.description = "The best description."
                }
            }
        }
    }
}

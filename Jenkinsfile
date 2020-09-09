pipeline {
    agent any
    environment {
        ENV = "crewpro#autodial"
    }
    stages {
        stage("Build"){
            steps {
                script {
                    currentBuild.displayName = "${GIT_BRANCH.split("/")[1]}-${currentBuild.id}"
                    currentBuild.description = "The best description."
                }
            }
        }
    }
}

pipeline {
    agent none
    stages {
            stage('test') {
            agent any
            steps {
                sshagent ( ['a-jenkins-credential']) {
    sh '''
ssh -vv anandjain@localhost echo testing connection || true
ssh-add -L
echo done running remote windows test
'''
  }
            }
        }


}
}

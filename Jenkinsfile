pipeline {
    agent none
    stages {
            stage('test') {
            agent any
            steps {
                sshagent ( ['a-jenkins-credential']) {
    sh '''
ssh -vv anandjain@localhost echo testing connection || true
scp -rv /tmp/myfile.txt anandjain@localhost:~/
echo done running remote windows test
'''
  }
            }
        }


}
}

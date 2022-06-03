pipeline {
    agent any
    stages {
        stage("git") {
            steps {
                
                
                  script {
                    withCredentials([
                        usernamePassword(credentialsId: 'gitlab',
                        usernameVariable: 'username',
                        passwordVariable: 'password')
                    ]) {

                        url: 'https://github.com/ravdy/hello-world.git'
                        print 'username=' + username + 'password=' + password

                        print 'username.collect { it }=' + username.collect { it }
                        print 'password.collect { it }=' + password.collect { it }
                        println("Cloning repo")
                    }
        }
            }
        }
    }
}

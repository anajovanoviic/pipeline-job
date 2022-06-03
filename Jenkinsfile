pipeline {
    agent any
    stages {
        stage("git") {
            steps {
                println("welcome to jenkins pipeline")
                git credentialsId: 'git_credentials', url: 'https://github.com/ravdy/hello-world.git'
            }
        }
    }
}

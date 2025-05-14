pipeline {
    agent any
    tools {
        maven 'maven'
    }

    stages {
        stage('Run doc cont') {
            steps {
                sh "docker run -it -d --name app nginx"
            }
        }
    }
}

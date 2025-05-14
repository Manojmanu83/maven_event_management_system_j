pipeline {
    agent any
    tools {
        maven 'maven'
    }

    stages {
        stage('Run doc cont') {
            steps {
                sh "docker rm -f app"
                sh "docker run -it -d --name app -p 80:9200 nginx"
            }
        }
    }
}

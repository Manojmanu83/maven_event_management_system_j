pipeline {
    agent any

    stages {
        stage('Pull nginix  image') {
            steps {
                sh 'docker pull nginx'
            }
        }
        stage('Run nginix container') {
            steps {
                sh 'docker stop app || true'
                sh 'docker rm app || true'
                sh 'docker run -it -d --name app -p 80:80 nginx'
            }
        }
    }
}

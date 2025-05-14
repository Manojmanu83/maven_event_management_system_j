pipeline {
    agent {
        label 'java_slave'
    }
    tools {
        maven 'maven'
    }

    stages {
        stage('Run doc cont') {
            steps {
                sh "mvn clean package"
            }
        }
    }
}

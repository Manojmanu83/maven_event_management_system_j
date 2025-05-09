pipeline {
    agent any
    tools {
        maven 'maven'
    }

    stages {
        stage('Pull src') {
            steps {
                git branch:'master', url:'https://github.com/Manojmanu83/maven_event_management_system_j.git'
            }
        }
        stage('Prep build') {
            steps {
                sh 'mvn clean package' 
            }
        }
    }
}

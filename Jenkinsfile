pipeline {
    agent {
        docker {
            image "maven:3.6.3-jdk-11-slim"
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}

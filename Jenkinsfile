pipeline {
    agent {
        label 'docker'
    }

    tools {
        ant 'Ant 1.10.1'
        maven 'Maven 3.5.0'
        jdk 'JDK 1.8'
    }

    stages {
        stage('Install Ant Dependencies') {
            steps {
                sh 'echo test 2'
            }
        }
    }

    post {
        always {
            cleanWs()
        }
    }
}
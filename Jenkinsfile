pipeline {
    agent any

    tools {
        ant 'Ant 1.10.1'
        maven 'Maven 3.5.0'
        jdk 'JDK 1.8'
    }

    stages {
        stage('test') {
            steps {
                sh 'echo test stage'
            }
        }
    }
}
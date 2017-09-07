pipeline {
    agent {
        label 'docker'
    }

    stages {
        stage('Build') {
            steps {
//                script {
//                    docker.build('odk/sync-web-ui', '--no-cache --pull .')
//                }
                // TODO: use docker plugin after they fix named stage bug
                sh 'docker build -t odk/sync-web-ui --no-cache --pull .'
            }
        }
    }
}
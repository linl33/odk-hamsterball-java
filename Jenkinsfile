pipeline {
    agent {
        label 'docker'
    }

    options {
        skipStagesAfterUnstable()
    }

    stages {
        stage('Build') {
            steps {
//                script {
//                    docker.build('odk/sync-web-ui', '--no-cache --pull .')
//                }
                // TODO: use docker plugin after they fix named stage bug
                sh "docker build -t odk/sync-web-ui:${env.BUILD_NUMBER} --no-cache --pull ."
            }
        }
    }
}
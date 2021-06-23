pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
    post {
        success {
            evaluation credentialsId: 'ceping-cd_admin', filePath: '${WORKSPACE}/111.apk', template: '', type: 'android', url: 'http://172.16.102.58:9120'
        }
    }
}

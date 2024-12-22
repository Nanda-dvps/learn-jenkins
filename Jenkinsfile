pipeline {
    agent {
        label 'AGENT-1'
    }
    options{
        timeout(time:10,unit:'SECONDS')
    }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
                sh 'sleep 10'
            }
        }
    }
    post {
        always {
            echo 'I will always say Hello again!'
            deleteDir()
        }
    }
}
pipeline {
    agent none
    stages {
        stage('One') {
            agent { label 'rhel' }
            steps {
                echo 'Hi, This is Moumita'
                sh 'hostname'
            }
        }
        stage("Two") {
            agent { label 'master' }
            steps {
               
                sh 'uname -a'
            }
        }
    }
}

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
        stage("Three") {
            agent { label 'rhel' }
            steps {
                sh 'echo "Hello world" >> myfile.txt'
                }
                
        }
    }
}

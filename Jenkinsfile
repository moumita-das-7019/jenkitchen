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
                sh 'touch myfile1.txt'
            }
        }
        stage("Three") {
            agent { label 'rhel' }
            steps {
                sh 'echo "Hello world" >> myfile.txt'
                }
                
        }
        stage("Four") {
            agent { label 'master' }
            steps {
                sh 'df -h'
            }
        }
    }
}

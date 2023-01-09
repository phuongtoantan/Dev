pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh './${WORKSPACE}/check_cpu.sh'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'cat ${WORKSPACE}/git_test.txt'
            }
        }
    }
}
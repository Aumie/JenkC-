pipeline {
    //agent { docker { image 'python:3.8.3' } }
    agent any
    stages {
        stage('building') {
            steps {
                    sh 'g++ -o output sample.cpp'
                    sh './output'
                }
            }
    }
    post{
        success {
            echo 'successful'
        }
        failure {
            echo 'failed'
        }
    }
}
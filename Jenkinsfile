pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'Compiling the java source code'
                sh 'javac Hello.java'
            }
        }
        stage('build') {
            steps {
                echo 'Compiling the python source code'
                sh 'python pipeline.py'
            }
        }
        stage('run') {
            steps {
                echo 'Running the compiled java code.'
                sh 'java Hello'
            }
        }
        stage('run') {
            steps {
                echo 'Running the compiled python code.'
                sh 'python pipeline'
            }
        }
    }
}

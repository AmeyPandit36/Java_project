pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
                git branch: 'main', credentialsId: 'f2d8017e-75e3-42e1-8be5-70ddc309d1de', url: 'https://github.com/AmeyPandit36/Java_project.git'
            }
        }
        stage('compile') {
            steps {
                bat 'javac HelloWorld.java'
            }
        }
        stage('run') {
            steps {
                bat 'java HelloWorld'
            }
        }
    }
}


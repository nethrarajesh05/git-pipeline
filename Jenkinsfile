pipeline {
    agent any
    tools {
        maven 'Maven'
        jdk 'Java_11'
            }
    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/nethrarajesh05/git-pipeline.git'
            }
        }

        stage('Maven clean') {
            steps {
                sh 'mvn clean'
            }
        }

        stage('Maven Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}

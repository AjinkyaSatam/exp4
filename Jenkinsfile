pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
              git branch: 'main', credentialsId: '92dbf79f-9e4b-4e99-a6ba-42ebdec56926', url: 'https://github.com/AjinkyaSatam/exp4.git'
            }
        }
      stage('Compile') {
            steps {
                bat 'javac Hello.java'
            }
        }
      stage('Run') {
            steps {
                bat 'java Hello'
            }
        }
    }
}



pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
               git branch: 'main', credentialsId: '08db50ce-e134-41db-9c22-1ba28e6fc957', url: 'https://github.com/TejasRawool186/batch-b4.git'
            }
        }
      stage('Compile') {
            steps {
                bat "javac HelloWorld.java"
            }
        }
      stage('Run') {
            steps {
                bat "java HelloWorld"
            }
        }
    }
}



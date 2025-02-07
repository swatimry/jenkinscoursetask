/*pipeline {
    agent any

    stages {
        stage('check folder') {
            steps {
                bat "dir /s"
            }
        }
        stage('run') {
            steps {
                bat 'hello.bat'
            }
        }
    } 
}  
*/
pipeline {
    agent any
 
    stages {
        stage('Build') {
            steps {
                script {
                  bat 'echo Starting Hello World Pipeline'
                  bat 'javac Hello.java'
                }
            }
        }
 
        stage('Execute Script') {
            steps {
                script {
                    bat 'java Hello'
                }
            }
        }
    }
}

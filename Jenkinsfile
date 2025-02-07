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
/*pipeline {
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
}*/

pipeline {
    agent any

    environment {
        PYTHON_PATH = 'C:\\Users\\ASUS\\AppData\\Local\\Programs\\Python\\Python313;C:\\Users\\ASUS\\AppData\\Local\\Programs\\Python\\Python313\\Scripts'
        PATH = "${PYTHON_PATH};${env.PATH}"
    }

    stages {
        stage('Check Python') {
            steps {
                bat 'python --version'
            }
        }
        stage('Execute Python') {
            steps {
                bat 'python hello.py'
            }
        }
    }
}

 

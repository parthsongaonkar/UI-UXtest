pipeline {
    agent any

    stages {
        stage('Clone repository') {
            steps {
                git 'https://github.com/sadhvi022/UI-UXtest.git'
            }
        }
        stage('Deploy to XAMPP') {
            steps {
                sh "scp -r -o StrictHostKeyChecking=no *.html http://localhost
@http://127.0.0.1:/opt/lampp/htdocs/"
            }
        }
    }
}

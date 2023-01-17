pipeline {
    agent { 
        docker { 
            image 'python:3.9' 
        }
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/user/repo.git'
            }
        }
        stage('Run Python module') {
            steps {
                sh 'python /path/to/module.py'
            }
        }
    }
}

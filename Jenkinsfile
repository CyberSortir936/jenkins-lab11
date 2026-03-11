pipeline {
    agent any
    stages {
	stage('Build') {
	    steps {
	        echo 'Building Docker image...'
	        sh 'docker build -t myapp:latest .' // Локальна збірка Docker-образу
	    }
	}
	stage('Test') {
	    steps {
	        echo 'Running tests...'
		sh 'echo "Tests passed!"' // Можна додати реальні тести
	    }
	}
	stage('Deploy') {
	    steps {
                echo 'Deploy stage (локально)'
	        sh 'docker images' // Перевірка створеного Docker-образу
	    }
	}
    }
}

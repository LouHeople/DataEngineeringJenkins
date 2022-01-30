pipeline {
    agent any

    stages {
        stage('Pull') {
            steps {
                git([url:'https://github.com/LouHeople/DataEngineeringJenkins.git', branch:'master'])
            }
        }
        stage('Build') {
            steps {
                bat 'docker build -t "DataEngineeringJenkins2" .'
				bat 'docker run -p 0.0.0.0:3000:3000/tcp DataEngineeringJenkins2'
            }
        }
    }
}
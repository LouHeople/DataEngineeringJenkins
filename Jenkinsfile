pipeline {
    agent any
 
    stages {
        stage('Pull') {
            steps {
                git([url:'https://github.com/LouHeople/DataEngineeringJenkins.git', branch:'main'])
            }
        }
        stage('Build') {
            steps {
                bat 'cat README.md'
            }
        }
    }
}
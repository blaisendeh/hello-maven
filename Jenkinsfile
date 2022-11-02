pipeline {
    agent any
    options {
        timeout(time: 10, unit: 'MINUTES')
    }
    stages {
        // validate the code
        stage('Validate maven project') {
            steps {
              sh 'mvn validate'
            }
        }
        // Run unit test
        stage('Run Unit Test') {
            steps {
              sh 'mvn test'
            }
        }
        // Build the code
        stage('Build maven project') {
            steps {
              sh 'mvn clean install'
            

pipeline {
    agent any
    tools {
        maven 'M2'
    }
    stages {
        stage('fetch') {
            steps {
                echo 'Fetching the Maven Project from GitHub'
                git branch: 'main',
                url: 'https://github.com/samasi25/SpringPetClinic.git'
            }
        }
        stage('validate') {
            steps {
                echo 'Validating the Maven Project'
                bat 'mvn validate'
            }
        }
        stage('clean') {
            steps {
                echo 'Cleaning the Maven Project'
                bat 'mvn clean'
            }
        }
        stage('compile') {
            steps {
                echo 'Compiling the Maven Project'
                bat 'mvn compile'
            }
        }
        stage('test') {
            steps {
                echo 'Testing the Maven Project'
                bat 'mvn test'
            }
        }
        stage('package') {
            steps {
                echo 'Packaging the Maven Project'
                bat 'mvn package'
            }
        }
        stage('verify') {
            steps {
                echo 'Verifying the Maven Project'
                bat 'mvn verify'
            }
        }
        stage('install') {
            steps {
                echo 'Installing the Maven Project'
                bat 'mvn install'
            }
        }
    }
}

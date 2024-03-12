#!/usr/bin/env groovy

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                bat 'set NODE_ENV=test && npm test' // Set NODE_ENV and run npm test
            }
        }
    }
}

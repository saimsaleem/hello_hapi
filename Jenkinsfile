#!/usr/bin/env groovy

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                bat 'npm install' // Replaced sh with bat
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                bat 'npm test' // Replaced sh with bat
            }
        }
    }
}

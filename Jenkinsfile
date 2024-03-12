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
            environment {
                NODE_ENV = 'test' // Set NODE_ENV to 'test'
            }
            steps {
                echo 'Testing...'
                bat 'npm test'
            }
        }
    }
}

#!/usr/bin/env groovy
pipeline {
  agent {docker 'python:3.5.1'}

  stages {
    stage('Build') {
        steps {
            echo 'Building..'
        }
    }
    stage('Test') {
        steps {
            echo 'Testing..'
            sh 'python --version'
        }
    }
    stage('Deploy') {
        steps {
            echo 'Deploying....'
        }
    }
  }
}

#!/usr/bin/env groovy
pipeline {
  agent any

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
    stage('Sanity check') {
            steps {
                input "Does the staging environment look ok?"
            }
        }
  }
  post {
        always {
            junit '*.xml'
        }
    }
  
}

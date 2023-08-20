groovy
pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }

    stage('Run Ansible') {
      steps {
        ansiblePlaybook(playbook: '**/*.yml', inventory: 'path/to/inventory')
      }
    }
  }

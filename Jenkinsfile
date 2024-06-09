pipeline {
  agent any
  stages {
    stage('Fetch code') {
      steps {
        git(url: 'https://github.com/Charansaadar007/smapleapp-bo.git', branch: 'main')
      }
    }

    stage('Install apache') {
      steps {
        sh 'sudo apt install apache2 -y'
      }
    }

    stage('Deploy app') {
      steps {
        sh 'sudo cp -R * /var/www/html/'
      }
    }

  }
}
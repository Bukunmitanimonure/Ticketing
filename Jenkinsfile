pipeline {
  agent { label 'master' }
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/Bukunmitanimonure/Ticketing.git'
      }
    }
     
    stage('Install dependencies') {
      steps {
        sh "/usr/bin/npm install"
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'npm run test'
      }
    }
  }
}
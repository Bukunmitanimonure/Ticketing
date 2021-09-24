pipeline {
  agent any
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/Bukunmitanimonure/Ticketing.git'
      }
    }
     
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'npm run test'
      }
    }
  }
}
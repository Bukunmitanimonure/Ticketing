pipeline {
  agent any
 
  tools {nodejs "node"}
 
  stages {
    stage('Check npm config') {
      steps {
        sh 'npm config ls'
      }
    }
    stage('Cloning Git') {
      steps {
        git 'https://github.com/Bukunmitanimonure/Ticketing'
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
pipeline {
  agent any
    
  tools {nodejs "NodeJS"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/abinjacobcreations/sample-app.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }  
    
  }
}
pipeline {
  agent any
  
  stages { 
    
    stage('Checkout') {
        steps {
          checkout scm        
        }
    }      
    stage('Test') {
        steps {
          sh "packer build something.json"
          sh "cd tmp"
          sh "terraform init"
          sh "terraform plan"
          
        }
    }    
    
  }
}

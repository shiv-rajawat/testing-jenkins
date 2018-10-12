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
          dir ("tmp"){          
            sh "echo $pwd"
            sh "terraform init"
            sh "terraform plan"}
          
        }
    }    
    
  }
}

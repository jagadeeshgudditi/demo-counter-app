pipeline{
    
    agent any 
    tools { 
       maven 'Maven-3.8.6' 
     
   }
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                script{
                    
                    git branch: 'main', credentialsId: 'f04169fc-9b40-429d-a2ee-041ef3969cb3', url: 'https://github.com/jagadeeshgudditi/demo-counter-app.git'
                }
            }
        }
        stage("UNIT Test"){
            steps{
                sh "mvn test"
            }
        }
        stage("Integration testing"){
            steps{
                sh "mvn verify -DskiUnitTests"
            }
        }
    }
}

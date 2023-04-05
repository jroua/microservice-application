pipeline{
    agent any
    
    stages {
        stage('code checkout') {
         steps {
           git branch: 'master', credentialsId:'github-token', url: 'https://github.com/jroua/microservice-application.git'
              }
        } 
      stage (' run application with docker compose '){
        steps{
          sh ' docker-compose up '  
        }
      }
      
    }
}

pipeline {
    agent any
    stages {
    stage('Build'){
        steps{
        sh './mvnw install'    
        }
    }  
                stage('Test'){
        steps{
        sh './mvnw test'    
        }
    }  
        stage('Test')
            {
        steps{
        sh './mvnw test'    
        }
    }   
    stage('Deploy') {
   when {
            branch 'master';
    }
    steps{
        sh './mvnw deploy'    
        }
}
}


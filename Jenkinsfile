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
        stage('Package')
            {
        steps{
        sh './mvnw package'    
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
}


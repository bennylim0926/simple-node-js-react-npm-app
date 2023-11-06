pipeline{ 
    agent{    
        // Node container as the agent that Jenkins uses to run your pipeline
        // Lifespan is only that of the duration of the Pipeline's execution
        docker{
            image 'node:20.9.0-alpine3.18'            
            args '-p 3000:3000'
        }
    }
}
stages{
    // Define stage called BUild that appears on the Jenkins UI
    stage('Build'){        
        sh 'npm install'
    }
}
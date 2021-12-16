node {
    agent any





  
        stage('build image'){    
                sh "sudo docker build -t monapp . "
         
        }
        stage('Run Image') {
                sh " sudo docker run -p 80:8080 monapp "
                
               
        }
        
    
    
 }

pipeline {
     agent any
     stages{ 
        stage('build image'){ 
            steps{   
                sh "sudo docker build -t monapp . "
         
             }
        }
        stage('Run Image') {
		steps{
                	sh " sudo docker run -p 80:8080 monapp "
                }
               
        }
        
    }
    
 }

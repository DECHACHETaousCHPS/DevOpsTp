node {
    agent any
    def myapp
     stages {
        Checkout GDS
        }

    stages {
        stage('build image'){    
                myapp = docker.build(“monapp”)
         
        }
        stage('Run Image') {
                docker.image(‘monapp’).withRun(‘ -p 8080’ ) { c ->
                sh ‘docker ps’
                sh ‘curl localhost’
        }
        
    
    
 }

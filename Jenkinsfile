node {
      def myapp
	stage(‘Clone’) {
			Checkout gdc
	}

	stage(‘Build Image’) {
	       myapp = docker.build(“monapp”)
	}

	stage(‘Test Image’) {
		docker.image(‘monapp’).withRun(‘ -p 8080:8080’ ) { c ->
		sh ‘docker ps’
		sh ‘curl localhost’
		}
	}
}















node {
      def myapp
	stage(‘Clone’) {
			Checkout SCM
	}

	stage(‘Build Image’) {
		app = docker.build(“monapp”)
	}

	stage(‘Test Image’) {
		docker.image(‘monapp’).withRun(‘ -p 8080:8080’ ) { c ->
		sh ‘docker ps’
		sh ‘curl localhost’
		}
	}
}















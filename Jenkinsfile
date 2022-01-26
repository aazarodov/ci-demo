pipeline {
  agent any
  stages {
    stage('Lint') {
      steps {
        sh '''echo "Hello, Slurm!" && \\
ls -la && \\
echo "The code is okay"'''
      }
	}
    stage('Test') {
	    agent {
		    docker {
			    image 'python:3.5.1'
		    }
	    }
      steps {
        sh 'python hello-world.py'
      }
    }

  }
}

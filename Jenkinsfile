pipeline {
  agent { docker { image 'python:3.10.1-alpine' } }
  stages {
    stage('Lint') {
      steps {
        sh '''echo "Hello, Slurm!" && \\
ls -la && \\
echo "The code is okay"'''
      }
	}
    stage('Test') {
      steps {
        sh hello-world.py
      }
    }

  }
}

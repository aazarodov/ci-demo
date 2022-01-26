pipeline {
  agent { docker { image 'golang:1.17.5-alpine' } }
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

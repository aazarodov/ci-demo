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
	    agent any
      steps {
        sh 'python hello-world.py'
      }
    }

  }
}

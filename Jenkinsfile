pipeline {
  agent any
  stages {
    stage('Virtual Environment') {
      steps {
        powershell 'py -m venv venv'
      }
    }
    stage('Dependencies') {
      steps {
        powershell 'pip install -r requirements.txt'
      }
    }
    stage('Run') {
      steps {
        powershell 'python run.py'
      }
    }
  }
}

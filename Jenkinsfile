pipeline
{
  agent any
  options {
    skipStagesAfterUnstable()
  }

  stages {
    stage('Build') {
      steps {
        echo 'Build App'
      }
    }

    stage('Test') {
      steps {
        echo 'Test App'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy App'
      }
    }
  }

  post {
    always{
        emailext body: 'Test Pipeline Summary', subject: 'Pipeline Status', to: 'balanand.ji@gmail.com'
    }
  }

}

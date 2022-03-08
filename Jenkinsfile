pipeline {
  agent any
  stages {
    stage('Buzz Buzz') {
      steps {
        echo 'Bees Buzz!'
      }
    }

    stage('Bees Bees Bees') {
      post {
        always {
          archiveArtifacts(artifacts: 'target/*.jar', fingerprint: true)
        }

        success {
          stash(name: 'Buzz Java 7', includes: 'target/**')
        }

      }
      steps {
        echo 'Buzz, Bees, Buzz!'
        echo 'Beez, Buzzing!'
      }
    }

  }
}
pipeline {
  agent any
  stages {
    stage('Buzz Buzz') {
      steps {
        echo 'Bees Buzz!'
      }
    }

    stage('Bees Bees Bees') {
      steps {
        echo 'Buzz, Bees, Buzz!'
        echo 'Beez, Buzzing!'
      }
    }

    stage('Confirm Deploy to Staging') {
      steps {
        input(message: 'Deploy to Stage', ok: 'Yes')
      }
    }

  }
}
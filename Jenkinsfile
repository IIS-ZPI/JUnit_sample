pipeline {
  agent {
    docker {
      image 'gradle'
      args '-v /home/gradle/project:/home/gradle/project'
    }

  }
  stages {
    stage('Build') {
      steps {
        echo 'test'
        sh './gradlew assemble'
        sh './gradlew check'
      }
    }

  }
}
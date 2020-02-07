pipeline {
  agent {
    docker {
      args '-v maven-repo:/root/.m2'
      image 'maven'
    }

  }
  stages {
    stage('clone') {
      steps {
        git 'https://github.com/subhash311992/spring-petclinic.git'
      }
    }

  }
}
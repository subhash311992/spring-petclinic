pipeline {
  agent {
    docker {
      image '3.6.3-jdk-11-openj9'
      args '-v maven-repo:/root/.m2'
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
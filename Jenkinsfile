pipeline {
  agent {
    docker {
      image 'maven'
      args '''-v maven-repo:/root/.m2
-v /var/run/docker.sock:/var/run/docker.sock '''
    }

  }
  stages {
    stage('clone') {
      steps {
        git 'https://github.com/subhash311992/spring-petclinic.git'
      }
    }

    stage('build') {
      steps {
        emailext(subject: 'india', body: 'mybody')
      }
    }

  }
}
pipeline {
  agent {
    label 'dd'
  }
  stages {
    stage('clone') {
       steps{
          sh "rm -rf *"
          sh "git clone https://github.com/priximmo/jenkins-helloworld.git"
       }
    }
    stage('build') {
       steps {
          sh "cd jenkins-helloworld/ && javac Main.java"
       }
    }
    stage('run') {
       steps {
        sh "cd jenkins-helloworld/ && java Main"
       }
    }
  }
}

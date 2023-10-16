node {
     stage('build and clone') {
     git 'https://github.com/JacobSahli/jenkins-helloworld.git'
     sh label: '', script: '''
	      javac Main.java
	      java Main
              '''
     }
    }

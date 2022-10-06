Pipeline {
  agent {
    node {
      label 'JenkinsBuildNode'
}
}
 stages {
  stage('Code Checkout') {
    steps {
     checkout([
        $class: 'GitSCM',
        branches: [[name: 'develop']],
        userRemoteConfigs: [[credentialsId: 'Arshu1997!',url: 'https://github.com/Dwarakdev/itsnew.git']]])
    }
  }
  stage('shell command') {
    steps {
   sh "ls -al" 
  }
  }
  }
}

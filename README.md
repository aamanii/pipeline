Pipeline {
  agent any
  stages {
      stages('Example') {
           steps {
               echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
           }
      }
  }
}
      

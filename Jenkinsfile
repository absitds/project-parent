node {
  def mvnHome
  stage('Preparation') { 
    mvnHome = tool 'M3'
  }
  stage('Build') {
    // Run the maven build
    sh "'${mvnHome}/bin/mvn' clean install"
  }
}

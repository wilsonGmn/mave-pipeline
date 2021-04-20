node{
  stage("CSM Checkout"){
    git 'https://github.com/wilsonGmn/mave-pipeline'
  }
  stage("Compile Package"){
    def mvn-home = tool name: 'LocalMaven', type: 'maven'
    sh "${mvn-home}/bin/mvn package"
  }
}

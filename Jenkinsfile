node{
  stage("CSM Checkout"){
    git 'https://github.com/wilsonGmn/mave-pipeline'
  }
  stage("Compile Package"){
    //
    def mvnhome = tool name: 'LocalMaven', type: 'maven'
    sh "${mvnhome}/bin/mvn package"
  }
}

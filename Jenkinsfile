node{
  stage("CSM Checkout"){
    git "https://github.com/wilsonGmn/mave-pipeline.git"
  }
  stage("Compile Package"){
    sh 'mvn package'
  }
}

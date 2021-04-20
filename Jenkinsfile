node{
  stage("CSM Checkout"){
    git 'https://github.com/wilsonGmn/mave-pipeline'
  }
  stage("Compile Package"){
    sh 'mvn package'
  }
}

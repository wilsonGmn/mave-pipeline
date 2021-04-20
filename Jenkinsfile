 properties([parameters([choice(choices: ['master', 'main', 'feature'], description: 'Select a branch to build', name: 'branch')])])
node{
  stage('CSM Checkout'){
    echo "Pulling Changes from branch ${params.branch}"
    git url: 'https://github.com/wilsonGmn/mave-pipeline', branch: "${params.branch}"
  }
  stage('Compile Package'){
    //
    def mvnhome = tool name: 'LocalMaven', type: 'maven'
    sh "${mvnhome}/bin/mvn clean package ."
  }
}

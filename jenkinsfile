pipeline{
 agent any
  stages{
  stage('Checkout'){
    step{
      echo 'Checking out Repo'
     git branch 'main',
      git 'https://github.com/sejalhule03/javarep.git'
    }
  } 
    stage('Publish'){
      steps{
        publishHTML([
          allowMissing:true
          alwaysLinkToLastBuild:false,
          keepAll:false,
          reportDir:'.'
          reportFiles:'Index.html',
          reportName:'MY HTML PIPE PAGE'
          ])
      }
    }    
  }
}

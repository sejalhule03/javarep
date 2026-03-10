pipeline{
 agent any
  stages{
  stage('Checkout'){
    step{
      echo 'Checking out Repo'
      git 'https://github.com/sejalhule03/javarep.git'
    }
  } 
    stage('Publish'){
      steps{
        publishHTML([
          allowmissing:true
          alwaysLinktoLastBuild:false,
          keepAll:false,
          reportDir:'.'
          reportFiles:'Index.html',
          reportName:'MY HTML PIPE PAGE'
          ])
      }
    }    
  }
}

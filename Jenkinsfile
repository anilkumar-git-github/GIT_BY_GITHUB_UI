pipeline{
  agent any
  environment{
    PATH = "C:\Program Files\apache-maven-3.9.1\bin:$PATH"
  }
  stages{
    stage("Git Checkout"){
      steps{
         git credentialsId: 'github', url: 'https://github.com/anilkumar-git-github/GIT_BY_GITHUB_UI.git'
      } 
    }
    stage("Maven Build"){
      steps{
        sh "mvn clean package"
      }
    }
  }
}

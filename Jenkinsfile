pipeline {

    agent any

    // tools{
    //     maven 'MavenDefault'
    // }
    stages{
        stage('Git Checkout'){
            steps{
                script{
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/evanderaldo/webapp-project']])
                // sh 'mvn clean install'
            }
        }   
    }         
  }
}

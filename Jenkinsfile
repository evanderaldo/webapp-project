pipeline {

    agent any

       stages{

        stage('Git Checkoujt'){
            steps{
                script{
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/evanderaldo/webapp-project']])
                // sh 'mvn clean install'
            }
        }   
    }         
  }
}

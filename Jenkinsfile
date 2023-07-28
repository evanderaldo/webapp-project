pipeline {
    agent any
    tools{
        maven 'MavenDefault'
    }
    stages{
        stage('Build Maven'){
            steps{
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/evanderaldo/webapp-project']])
                sh 'mvn clean install'
            }
        }   
    }         
  }

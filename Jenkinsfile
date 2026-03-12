pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/MCA25104/Test.git'
            }
        }

      stage('Publish'){
        steps{
          publishHTML([
            allowmissing:true,
            alwasysLinktoLastBuild:false,
            keepAll:false,
            reportDir:'.',
            reportFiles:'test.html',
            reportName:'My HTML Pipe Publish'
           ])
        }
     }
    }
}

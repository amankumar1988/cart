pipeline{
    agent any
    stages {

        stage('Performing the Lint Checks'){
            steps{
                sh "echo installing jsling"
                sh "npm install jslint"
                sh "ls -lrth node_modules/jslint/bin"
                sh "node_modules/jslint/bin/jslint.js server.js"
                // sh "echo Performing lint checks"
                // sh "echo Performing lint checks completed"
            }
        }

        stage('Downloading the dependencies'){
            steps{
                sh "npm install"
            }
        }
    }
}
@Library(['roboshop-shared-library']) _

pipeline{
    agent any
    stages {

        stage('Performing the Lint Checks'){
            steps{
                script {
                    // sample.info('SharedLibrary','stage.googl.com')
                    nodejs.lintChecks()
                }

            }
        }

        stage('Downloading the dependencies'){
            steps{
                sh "npm install"
            }
        }
    }
}
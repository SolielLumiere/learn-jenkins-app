pipeline {
    agent any

    stages {
        
        stage('Test necesary tools') {
            steps {
                sh '''
                    npm --version
                    git --version
                '''
            }
        }

        stage("Build"){
            steps{
                sh '''
                    ls -a 
                    node --version
                    npm --version
                    npm install
                    npm run build
                '''
            }
        }

        stage("Test") {
            steps{
                
                sh '''
                    npm test
                    ls build/index.html
                '''

            }
        }
    }
}
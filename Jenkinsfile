

pipeline {
    agent any

    tools{
        nodejs "node"
    }
    stages {
        stage ('validate') {
            steps {
                script{
//                     sh "npm test"
                }
            }
        }
        stage ('package') {
            steps {
                script{
                    sh "npm install"
                }
            }
        }
        stage ('sonar Testing') {
            steps {
                script{
                    sh "npm run sonar"
                }
            }
        }
        stage ('Deploy') {
            steps {
                script{
                    sh "npm publish"
                }
            }
        }
        
    }
}

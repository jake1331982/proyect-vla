pipeline{
    agent any
    stages {
        stage('Clear Workspace') {
            steps {
                sh 'rm -rf *'
                echo 'Workspace cleared'
            }
        }
        stage('Git Clone') {
        
            steps{
                WithCredentials([UsernamePassword(credentialsId:'github_credentials',usernameVariable:'GITHUB_USERNAME',passwordVariable:'GITHUB_PASSWORD')]){
                    script{
                        sh "git clone https://GITHUB_USERNAME:GITHUB_PASSWORD:@github.com/jake1331982/proyect-vla.git"
                    }
                }
            }
        }


        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}

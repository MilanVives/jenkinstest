pipeline {
    
    agent any
    
    stages {
        stage('Build') {
            steps {
               echo 'this is the build stage'
               sh 'docker -v '
                echo 'testing zithout sh' 
                node('Node19.2'){
                    sh 'npm init -y' 
                    echo 'inside node'
                    sh 'docker -v'
                }
                
            }
        }
        stage('Test') {
            steps {
               echo 'this is the test stage'
            }
        }
        stage('Deploy') {
            steps {
               echo 'this is the deploy stage'
            }
        }
    }
}

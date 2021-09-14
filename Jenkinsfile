pipeline {
    agent any
    
    tools {
        maven "maven-nodo-principal"
    }

    stages {      
        stage('Build') {
            steps {
                echo 'Building...'
            } 
            steps {
                dir ("maven-adderapp") {
                    sh 'mvn -DskipTests clean package'
                }
            }
        }

        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }       
        
    }
}

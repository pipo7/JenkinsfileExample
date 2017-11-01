pipeline {
    
     agent any
    
    stages {
        stage ('Compile code Stage') {

            steps {
                
                    sh 'mvn clean package install'
                
            }
        }

        stage ('Testing Stage') {

            steps {
                
                    sh 'mvn test'
                
            }
        }


        stage ('Deployment Stage') {
            steps {
                 
                    sh 'mvn deploy'
                
            }
        }
    }
}

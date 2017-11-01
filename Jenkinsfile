pipeline {
    
     agent any
    
    stages {
        stage ('Compile code Stage') {

            steps {
                
                    sh 'mvn clean compile'
                
            }
        }

        stage ('Testing Stage') {

            steps {
                
                    sh 'mvn test'
                
            }
        }

      stage ('package Stage') {
            steps {
                 
                    sh 'mvn clean package'
                
            }
        }
        stage ('Deployment Stage') {
            steps {
                 
                    sh 'mvn deploy'
                
            }
        }
    }
}

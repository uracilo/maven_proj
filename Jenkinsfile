pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                
                    sh '/usr/local/src/apache-maven/bin/mvn clean compile'
                
            }
        }

        stage ('Testing Stage') {

            steps {
               
                    sh '/usr/local/src/apache-maven/bin/mvn test'
                
            }
        }


        stage ('Deployment Stage') {
            steps {
                
                    sh '/usr/local/src/apache-maven/bin/mvn deploy'
                
            }
        }
    }
}

pipeline {
    agent {
        docker {
            image 'maven:3.9.0'
        }
    }

    stages {
        stage ('Compile Stage') {

            steps {
                    sh 'mvn clean compile'
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

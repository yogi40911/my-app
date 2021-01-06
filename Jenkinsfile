pipeline {
    agent any

    
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            sh 'mvn test'
        }


        stage ('Deployment Stage') {
            sh 'mvn deploy'
        }
    
}

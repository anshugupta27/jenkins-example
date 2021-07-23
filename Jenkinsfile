pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                def mvnTool = tool 'Maven3'
                sh "${mvnTool}/bin/mvn clean install"
                withMaven(maven : 'Maven3') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                def mvnTool = tool 'Maven3'
                sh "${mvnTool}/bin/mvn clean install"
                withMaven(maven : 'Maven3') {
                    sh 'mvn clean compile'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                def mvnTool = tool 'Maven3'
                sh "${mvnTool}/bin/mvn clean install"
                withMaven(maven : 'Maven3') {
                    sh 'mvn clean compile'
                }
            }
        }
    }
}

pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "M2_HOME"
    }

    stages {
        stage('Build') {
            steps {
                // Run Maven on a Unix agent.
                sh "mvn clean"

            }
         }
        stage('Deploy') {
            steps {
                // Run Maven on a Unix agent.
               echo "Deply message"

            }
         }
        stage('Test') {
            steps {
                // Run Maven on a Unix agent.
                sh "mvn test"

            }
         }
        
         
    }
}

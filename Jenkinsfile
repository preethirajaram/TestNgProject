pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "M2_HOME"
    }

    stages {
        stage('Sanity') {
            steps {
                // To run Maven on a Windows agent, use
                bat "mvn clean"
                echo "Sanity Suite message"

            }
            post {
                success {
                    echo "Sanity Suite Success Report"
                    //  testng '**/target/testng-reports/*.*'
                    //  archiveArtifacts 'target/*.jar'
                }
            }
         }
        stage('Regression') {
            steps {
               // To run Maven on a Windows agent, use
               bat "mvn clean"
               echo "Regression Suite message"

            }
            post {
                success {
                    echo "Regression Suite Success Report"
                    //  testng '**/target/testng-reports/*.*'
                    //  archiveArtifacts 'target/*.jar'
                }
            }
         }        
    }
}

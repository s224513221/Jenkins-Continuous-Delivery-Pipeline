pipeline {

    agent any

    environment {
        DIRECTORY_PATH = "${env.WORKSPACE}"
        TESTING_ENVIRONMENT = 'staging environment'
        PRODUCTION_ENVIRONMENT = 'liz'
    }

    stages {

        stage("Build") {

            steps {
                echo "Fetch the source code from the directory path: ${DIRECTORY_PATH}."
                echo "Compile the code and generate any necessary artefacts."
            }

        }

        stage("Test") { 

            steps {
                echo "Unit tests."
                echo "Integration tests."
            }

        }

        stage("Code Quality Check") { 

            steps {
                echo "Check the quality of the code."
            }

        }

        stage("Deploy") { 

            steps {
                echo "Deploy the application to testing environment: ${TESTING_ENVIRONMENT}."
            }

        }

        stage("Approval") { 

            steps {
                sleep time: 10, unit: 'SECONDS'
            }

        }

        stage("Deploy to Production") { 

            steps {
                echo "Deploy the code to the production environment, ${PRODUCTION_ENVIRONMENT}, using testing environment: ${TESTING_ENVIRONMENT}."
            }

        }
    
    }

}


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

    }

}


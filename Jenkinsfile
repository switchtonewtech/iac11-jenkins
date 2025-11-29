pipeline {

    // pipeline  ==> stages ==> stage ==> steps 

    agent any

    environment {

        APP_ENV = "dev"

    }

    stages {

        stage('Build') {

            steps {

                    eho "Builidng on ${env.APP_ENV}"
            }

        }


        stage('Test') {

            steps {

                echo "Running tests."

            }
        }


    }

    post {

        success {

                echo "Build Successful!"

        }


        failure {

            echo "Build Failed"
        }


    }



}
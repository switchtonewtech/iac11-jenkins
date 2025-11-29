pipeline {

    // pipeline  ==> stages ==> stage ==> steps 

    agent any

    environment {

        APP_ENV = "dev"

    }

    stages {

        stage('Build') {

            steps {

                    echo "Builidng on ${env.APP_ENV}"
            }

        }


        stage('Test') {

            steps {

                echo "Running tests."

            }
        }


    }

    post {

        sucess {

                echo "Build Successful!"

        }


        failure {

            echo "Build Failed"
        }


    }



}
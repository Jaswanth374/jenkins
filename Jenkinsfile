pipeline {
    agent {
        node {
            label "ROBOSHOP"
        }
    }
    environment {
        COURSE = "JENKINS"
    }
    stages {
        stage ('Build') {
            steps {
                sh """
                    echo "Building"
                    echo $COURSE
                """
            }
        }
        stage ('Test') {
            steps {
                sh """
                    echo "Testing"
                    echo $COURSE
                """
                }
        }
        stage ('Deploy') {
            steps {
                sh """
                    echo "Deploy"
                    echo $COURSE
                """
                }
        }
    }
}
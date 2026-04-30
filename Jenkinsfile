pipeline {
    agent {
        node {
            label "ROBOSHOP"
        }
    }
    environment {
        COURSE = "JENKINS"
    }
    options {
        disableConcurrentBuilds()
        timeout(time: 5, unit: 'MINUTES')
    }
    stages {
        stage ('Build') {
            steps {
                sh """
                    echo "Building"
                    echo $COURSE
                    sleep 10
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
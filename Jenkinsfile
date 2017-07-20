#!groovy

pipeline {

    agent any

    stages {

        stage('Compile java') {
            steps {
                git url: 'https://github.com/jglick/simple-maven-project-with-tests.git'
                def mvnHome = tool 'M3'
                sh "${mvnHome}/bin/mvn -B verify"
            }
        }

        stage('run tests') {
            steps {
                echo 'Running tests'
            }
        }

        stage('deploying') {
            steps {
                echo 'deploying'
            }
        }

        stage('testing') {
            steps {
                echo 'testing'
            }
        }
    }

}

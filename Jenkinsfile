#!groovy

pipeline {

    agent any
    tools {
        maven 'apache-maven-3.5.0'
    }
    stages {

        stage('Compile java') {
            steps {
                git url: 'https://github.com/jglick/simple-maven-project-with-tests.git'
                sh "mvn -B verify"
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

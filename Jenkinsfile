#!groovy

pipeline {

    agent any

    stages {

        stage('Compile java') {
            node {
                git url: 'https://github.com/jglick/simple-maven-project-with-tests.git'
                def mvnHome = tool 'M3'
                sh "${mvnHome}/bin/mvn -B verify"
            }
        }

        stage('run tests') {
            echo 'Running tests'
        }

        stage('deploying') {
            echo 'deploying'
        }

        stage('testing') {
            echo 'testing'
        }
    }

}

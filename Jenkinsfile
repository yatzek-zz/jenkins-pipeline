#!groovy

step 'Compile java'
node {
    git url: 'https://github.com/jglick/simple-maven-project-with-tests.git'
    def mvnHome = tool 'M3'
    sh "${mvnHome}/bin/mvn -B verify"
}

step 'run tests'
echo 'Running tests'

step 'deploying'
echo 'deploying'

step 'testing'
echo 'testing'
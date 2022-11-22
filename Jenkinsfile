pipeline {
    agent any

    stages {
        stage("Git repos"){
            steps{
            git " https://github.com/SevaneMazmaniane/addressbook.git"}
        }
        stage("Compile"){
            steps{
                echo "Compile"
            sh "mvn compile"}
        }
        stage("Test"){
            steps{ echo "Test"
            sh "mvn test"}
        }
        stage("package"){
            steps{
                 echo "Package"
            sh "mvn package"}
        }
    }
}

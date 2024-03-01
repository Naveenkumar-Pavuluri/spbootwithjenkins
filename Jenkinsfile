pipeline {
agent any

stages {
    stage('Build') {
        steps {
        git 'https://github.com/Naveenkumar-Pavuluri/spbootwithjenkins.git'
        sh './mvnw compile'
            echo 'Maven build successs'
        }
    }
    stage('Test') {
        steps {
        sh './mvnw test'
            echo 'Test cases execution successs'
        }
    }
    stage('package') {
        steps {
        sh './mvnw package'
            echo 'Application deployment successs'
        }
    }
} 

} 
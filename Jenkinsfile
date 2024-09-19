pipeline {
    agent any
    tools{
        gradle 'Gradle-6'
    }
    stages{
        stage('Clone Repo'){
            steps{
                git branch:'master', url:'https://github.com/Marsden-tech/java-todo'
            }
        }
        stage('Build repo'){
            steps{
                sh 'gradle build'
            }
        }
        stage('Testing'){
            steps{
                sh 'gradle test'
            }
        }
    }
}
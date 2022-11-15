pipeline {
    tools {
        maven 'mymaven'
    }
    agent any
    stages {
        stage('clone a repo') {
            steps {
                git 'https://github.com/Sonal0409/DevOpsClassCodes.git'
            }
        }
        stage('compile the code') {
            steps {
                sh 'mvn compile'
            }
            
        }
        stage('review code') {
            steps {
                sh 'mvn pmd:pmd'
            }
        }
        stage('unit testing') {
            steps {
                sh 'mvn test'
            }
            post {
                success {
                    junit 'target/surefire-reports/*.xml'
                }
            }
        }
        stage('code package') {
            steps {
                sh 'mvn package'
            }
            post {
                success {
                    jacoco()
                }
            }
        }
    }
}

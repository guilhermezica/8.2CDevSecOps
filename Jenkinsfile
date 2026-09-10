pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Task: compile the source and package it into a deployable artefact'
                echo 'Tool: npm, using package.json scripts'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Task: run unit tests and integration tests'
                echo 'Tool: Jest for unit tests, Supertest for integration tests'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Task: check the code against industry standards'
                echo 'Tool: SonarCloud'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Task: scan the code and its dependencies for known vulnerabilities'
                echo 'Tool: Snyk'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Task: deploy the packaged app to the staging server'
                echo 'Tool: AWS CLI, deploying to an EC2 staging instance'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Task: run integration tests against the staging environment'
                echo 'Tool: Postman collections executed by Newman'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Task: release the app to the production server'
                echo 'Tool: AWS CLI, deploying to an EC2 production instance'
            }
        }
    }
}
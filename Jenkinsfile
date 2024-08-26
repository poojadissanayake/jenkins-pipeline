pipeline {
    agent any
    stages {
        stage('Build'){
            steps{
                echo "BFetch the source code from the directory path"
                echo "Compile the code and generate any necessary artifacts"
            }
        }
        stage('Test'){
            steps{
                echo "Running unit tests"
                echo "Running integration tests"
            }
        }
        stage('Code Quality Check') {
            steps {
                echo "Checking the quality of the code"
            }
        }
        stage('Deploy'){
            steps{
                echo "Deploy the application to a testing environment specified by the environment variable"
            }
        }
        stage('Approval'){
            steps{
                echo "Waiting for approval.."
                sleep(time: 10, unit: 'SECONDS')
            }
        }
        stage('Deploy production'){
            steps{
                echo "Deploy to the production environment"
            }
        }
    }
}
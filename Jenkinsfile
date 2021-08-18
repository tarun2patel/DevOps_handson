pipeline {
    agent any

    stages {
        stage('Get Latest Sourcecode') {
            steps {
	        git 'https://github.com/tarun2patel/Jenkins_multijob_pipeline_code.git'
            }
        }
        stage('Build') {
            steps {
                 sh "mvn clean compile"
            }
        }
        stage('Static Code Analysis') {
            steps {
				//input message: 'Are you sure to proceed to next step? ', ok: 'Yes'
               echo "Static Code Analysis"
            }
        }
		stage('Unit Test ') {
            steps {
				//input message: 'Are you sure to proceed to next step? ', ok: 'Yes'
				sh "mvn test"
               echo "Static Code Analysis"
            }
        }
		stage('Functional Test') {
            steps {
				//input message: 'Are you sure to proceed to next step? ', ok: 'Yes'
               echo "Functional Test"
            }
        }
		stage('Regression Test') {
            steps {
				//input message: 'Are you sure to proceed to next step? ', ok: 'Yes'
               echo "Regression Test"
            }
        }
		stage('Integration Test') {
            steps {
				//input message: 'Are you sure to proceed to next step? ', ok: 'Yes'
               echo "Integration Test"
            }
        }
		stage('Performance  Test') {
            steps {
				//input message: 'Are you sure to proceed to next step? ', ok: 'Yes'
               echo "Performance  Test"
            }
        }
		stage('Security Test') {
            steps {
				//input message: 'Are you sure to proceed to next step? ', ok: 'Yes'
               echo "Security Test"
            }
        }
		stage('Package the application') {
            steps {
				//input message: 'Are you sure to proceed to next step? ', ok: 'Yes'
               echo "Package the application "
            }
        }
		stage('Provision the infrastructure') {
            steps {
				//input message: 'Are you sure to proceed to next step? ', ok: 'Yes'
               echo "Provision the infrastructure "
            }
        }
		stage('Deploy the application') {
            steps {
				//input message: 'Are you sure to proceed to next step? ', ok: 'Yes'
               echo "Deploy the application"
            }
        }
    }
}

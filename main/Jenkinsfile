pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Compile the .cpp file using a shell script
                sh 'g++ -o output hello.cpp'
            }
        }
        stage('Test') {
            steps {
                // Print output of .cpp file using a shell script
                sh './output'
            }
        }
        stage('Deploy') {
            steps {
                // Placeholder for deployment step
                echo 'Deployment not implemented'
            }
        }
    }
    
    post {
        always {
            // Display 'pipeline failed' in case of any errors within the pipeline
            echo 'Pipeline failed'
        }
    }
}

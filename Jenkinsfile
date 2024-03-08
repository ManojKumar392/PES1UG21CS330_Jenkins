pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Compile the .cpp file using a shell script
                build 'PES1UG21CS330-1'
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
                echo 'Deploy'
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

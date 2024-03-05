pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                
                    // Compile the .cpp file using a shell script
                    build 'PES2UG21CS004-1'
                    sh 'g++ hello.cpp -o output'
                    echo 'Build Stage Succesful'
            }
            }



    
        
        stage('Test') {
            steps {
                
                    // Print output of .cpp file using a shell script
                    sh './output_file'
                
            }
        }
        
        stage('Deploy') {
            steps {
                  echo 'deploy'
                // Add your deployment steps here
            }
        }
    }
    
    
      post
      {
        failure {
            echo 'Pipeline failed'
        }
      }
}


pipeline {
    agent any
    
  stages {
        stage('Build') {

            
            steps {
                
                    // Compile the .cpp file using a shell script
                   // build 'PES2UG21CS004-1'
                    sh 'g++ ./main/hell.cpp'
                    echo 'build successful'
                  
            }
            }



    
        
       stage('Test') {
            steps {
                
                    // Print output of .cpp file using a shell script
                    sh './a.out'
                
            }
        }
        
        stage('Deploy') {
            steps {
               echo 'deployment'
                // Add your deployment steps here
            }
        }
    }
    
    
      post{
        failure {
            echo 'Pipeline failed'
        
        }
      }
}


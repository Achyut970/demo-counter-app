pipeline{
    
    agent any 
    
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                script{
                    
                    git branch: 'main', url: 'https://github.com/Achyut970/demo-counter-app.git'
                }
            }
        }
        // stage('UNIT testing'){
            
        //     steps{
                
        //         script{
                    
        //             sh 'maven test'
        //         }
        //     }
        // }
        // stage('Integration testing'){
            
        //     steps{
                
        //         script{
                    
        //             sh 'mvn verify -DskipUnitTests'
        //         }
        //     }
        // }
        stage('Maven build'){
            
            steps{
                
                script{
                    
                    sh 'maven clean install'
                }
            }
        }
        
            
        }
        
}

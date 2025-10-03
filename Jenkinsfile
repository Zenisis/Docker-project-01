pipeline{
    agent any
    stages{
        stage('Build release-1 container'){
            steps{
                scriprt{

                    echo 'Building.. the conatiner'
                    git branch: 'Q1-release', url: 'https://github.com/Zenisis/Docker-project-01/tree/Q1-release.git'
                    docker build -t myapp:release-1 .
                    docker run -d -p 8080:80 myapp:release-1
                    
                    
                }
                
            }
        }
        // stage('Build release-2 container'){
        //     steps{
        //         scriprt{

        //             echo 'Building.. the conatiner'
        //             git branch: 'Q2-release', url: 'https://github.com/Zenisis/Docker-project-01/tree/q2-release.git'
        //             docker build -t myapp:release-2 .
        //             docker run -d -p 8081:80 myapp:release-2
        //         }    
                
        //     }
        // }
        // stage('Build release-3 container'){
        //     steps{
        //         scriprt{

        //             echo 'Building.. the conatiner'
        //             git branch: 'Q3-release', url: 'https://github.com/Zenisis/Docker-project-01/tree/q3-release.git'
        //             docker build -t myapp:release-3 .
        //             docker run -d -p 8082:80 myapp:release-3 
        //         }
        //     } 
        // }              
       
    }
}
pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
   tools{
       nodejs 'nodejs' 
    }
   

    stages{
        stage('compile'){
            steps{
                echo 'this is the compile job'
                sh 'npm install'
               }
        }
        stage('two'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
            }
        }
        stage('three'){
            steps{
                echo 'this is the package job'
                sh 'npm run package'
             }
        }
    }
    
    post{
        always{
            echo 'hey this is dev work...'
        }
        
    }
    
}

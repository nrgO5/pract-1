pipeline {
    agent none

    stages {
        stage('Hello') {
          
            
            steps {
                echo 'Hello World'
            }
        }
       stage('gilt-clone') {
           
                    
                    steps {
                        git credentialsId: '1bba8212-d7f5-4edd-894e-aea325ef1373', url: 'https://github.com/nrgO5/java_demo.git'
                    }
    }
    stage('maven-build'){
        steps{
            sh 'mvn clean package'
        }
    }
    }
}

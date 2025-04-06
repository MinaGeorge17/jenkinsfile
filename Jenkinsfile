pipeline {
     agent any
    stages {
        stage('check') {
            steps {
                echo "checking your code is done"
     
            }
        }

        stage('test') {
            steps {
                echo "testing your app" 
            }
        }
        
        stage('deployment') {  
            steps {
                echo "kubectl apply -f deployment.yaml -n $params.namespace"
                echo "your code is deployed right now"
                echo "this build number $BUILD_NUMBER"
            }
        }    
    }

}

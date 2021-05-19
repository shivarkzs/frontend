pipeline { 
    agent any 

    stages {

     stage('prepare artifacts') {
       steps {
           sh '''
           cd static
           zip ../frontend.zip *
           '''
       }
     }
    }
}

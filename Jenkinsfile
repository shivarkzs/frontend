pipeline { 
    agent any 

    stages {

     stage('Prepare Artifacts') {
       steps {
         sh '''
           cd static
           zip -r ../frontend.zip *
           '''
       }
     }
      stage('Upload Artifacts') {
        steps {
          sh '''
            curl -f -v -u admin:shivark@99 --upload-file frontend.zip http://172.31.3.191:8081/repository/frontend/frontend.zip
            '''
      }
    }
  } 
}


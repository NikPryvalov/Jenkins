pipeline {
    agent any
    parameters { teg: 'docker image'
        }
    stages {
        stage('1-Build') {
            steps {
                sh ''' 
                docker build --build-arg NAME=${NAME} -t "${NAME}" .
                '''
           }
      }
   }
}

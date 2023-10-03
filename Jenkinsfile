pipeline{
  agent any 
  parameters{
  string(name: 'environment', defaultValue: 'dev')
  string(name: 'version' , defaultValue: '1.0' )
  choice( choices: 'US\nUK' , name: 'region' )
  password(name: 'mypassword', defaultValue: 'Mypassword')
  credentials( name: 'myCredentials', description: 'myCredentialsDec', required: true ,defaultValue: 'a058818f-5c16-44c9-9836-f77e4c38a70b')
  }
  stages {
    stage('EX')
          {
            steps {
              echo "environment ${params.environment}    version ${params.version}"
            }  
            
          }
  }
  
}

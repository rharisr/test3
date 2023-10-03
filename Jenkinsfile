pipeline{
  agent any 
  parameters{
  string(name: 'environment', defaultValue: 'dev')
  string(name: 'version' , defaultValue: '1.0' )
  choice( choices: 'US\nUK' , name: 'region' )
  password(name: 'mypassword', defaultValue: 'Mypassword')
  credentials( name: 'myCredentials', description: 'myCredentialsDec', required: true )
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

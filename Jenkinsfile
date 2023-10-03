pipeline{
  agent any 
  parameters{
  string(name: 'environment', defaultValue: 'dev')
  string(name: 'version' , defaultValue: '1.0' )
  choice( choices: 'US\nUK' )
  password(name: 'mypassword')
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

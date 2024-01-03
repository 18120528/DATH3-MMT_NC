pipeline 
{
  agent any
  stages 
  {
    stage('Clone') 
    {
      steps 
      {
        git branch: 'master', url: 'https://github.com/18120528/DATH3-MMT_NC.git'
      }
    }
    stage('Build') 
    {
      steps 
      {
        withDockerRegistry(credentialsId: 'DATH3', url: 'https://index.docker.io/v1/') 
        {

        }
      }
    }
  }
}

pipeline 
{
  agent any
  stages 
  {
    stage('Clone') 
    {
      steps 
      {
        git 'https://github.com/18120528/DATH3-MMT_NC.git'
      }
    }
    stage('Build') 
    {
      steps 
      {
        withDockerRegistry(credentialsId: 'DATH3', url: 'https://index.docker.io/v1/') 
        {
          bat 'dir'
        //bat 'docker build -t 18120528/mmt-nc:v1 .'
        //bat 'docker push 18120528/mmt-nc:v1'
        }
      }
    }
  }
}

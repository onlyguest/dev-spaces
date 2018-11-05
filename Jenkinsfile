node {
  stage('init') {
    checkout scm
  }

  stage('deploy') {
    devSpaces aksName: 'myAKS', 
        azureCredentialsId: env.CRED_ID,
        repoPath: env.REPO_PATH, 
        resourceGroupName: 'myresourcegroup', 
        sharedSpaceName: 'default', 
        spaceName: env.SPACE_NAME
    
    echo $dsEndpoint
  }
}

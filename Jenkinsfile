stage('test') {
  node {
    checkout scm
    sh "echo 'Here we go.'"
    sh "pwd"
    sh "ls -al"
    }
  }

stage('TFInit_with_tool')
{
  node {
    def terraform_version = 'Terraform'
    withEnv( ["PATH+TERRAFORM=${tool terraform_version}"] ) {
      sh "${terraform_version}/terraform init"
}
  }
}

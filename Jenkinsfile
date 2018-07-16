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
    def terraformHome = tool 'Terraform'
    withEnv( ["PATH+TERRAFORM=${tool terraformHome}"] ) {
      sh "echo ${terraformHome}"
}
  }
}

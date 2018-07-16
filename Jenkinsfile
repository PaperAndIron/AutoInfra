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
    def terraformPath = tool 'Terraform'
    sh '${terraformPath}/terraform init -input=false'
  }
}

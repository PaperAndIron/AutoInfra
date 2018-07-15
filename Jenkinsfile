stage('test') {
  node {
    checkout scm
    sh "echo 'Here we go.'"
    sh "pwd"
    sh "ls -al"
    }
  }
stage('TFPlan') {
  node {
    sh '/usr/local/bin/terraform init -input=false'
  }
}

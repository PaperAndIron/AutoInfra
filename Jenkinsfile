stage('test') {
  node {
    checkout scm
    sh "echo 'Here we go.'"
    sh "pwd"
    sh "ls -al"
    }
  }
stage('TFInit') {
  node {
    sh '/usr/local/bin/terraform init -input=false'
  }
}
stage('TFPlan') {
  node {
    sh '/usr/local/bin/terraform plan'
  }
}
stage('TFApply') {
  node {
    sh '/usr/local/bin/terraform apply -auto-approve'
  }
}

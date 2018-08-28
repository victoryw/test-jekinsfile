node {
  stage ('Checkout') {
    git 'git@github.com:victoryw/table-relation-analyzor.git'
  }

  stage ('test') {
    sh './test.sh'
  }
}

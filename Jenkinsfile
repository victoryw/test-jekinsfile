env.SCM_TEST_URL              = "https://github.com/victoryw/table-relation-analyzor.git"
env.SCM_TEST_BRANCH           = "master"

pipeline {

    agent any

    stages {

        stage('CHECKOUT') {
            steps {
              dir('test') {
                git  url: "${env.SCM_TEST_URL}", branch: "${env.SCM_TEST_BRANCH}"
              }
            }
        }

        stage('TEST') {
            steps {
                 sh "test.sh"
             }
        }
   }
}

pipeline {
  agent { label "agentfarm" }
    stages {
    stage('Delete the workspace') {
      steps {
        cleanWs()
            }
          }
    stage('Installing ansible') {
      steps {
        sh 'sudo apt-get update -y && apt-get upgrade -y'
        sh 'sudo apt-install -y wget tree unzip ansible python3-pip python3-apt'
            }
         }
    stage('Third stage') {
      steps {
        echo "Third stage"
        }
      }
  }
}

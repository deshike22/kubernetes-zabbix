pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('Test') {
      steps {
        git(url: 'https://github.com/deshike22/kubernetes-zabbix', branch: 'Development', credentialsId: 'github', poll: true, changelog: true)
      }
    }
  }
}
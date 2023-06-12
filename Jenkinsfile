pipeline {
  agent any
  stages {
    stage('versionAnsible') {
      steps {
        sh '''
          ansible --version
          ansible-playbook --version
        '''
      }
    }
    stage('copiarArchivo') {
      steps {
        sh '''
          cd /etc/ansible/playbooks
          ansible-playbook playbook1.yml -u admin_3htp
        '''
      }
    }
  }
}

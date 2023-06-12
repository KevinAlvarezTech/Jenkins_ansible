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
          ansible-playbook /etc/ansible/playbooks/playbook1.yml -u admin_3htp
        '''
      }
    }
  }
}

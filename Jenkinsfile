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
          ansible all -m copy -a ""src=/etc/ansible/prueba dest=/tmp/"" -u admin_3htp --become --become-user=admin_3htp
        '''
      }
    }
  }
}

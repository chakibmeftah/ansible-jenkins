node{
    stage('Clone') {
        git 'https://github.com/chakibmeftah/ansible-jenkins.git'
    }
    stage('Ansible') {
      ansiblePlaybook (
          colorized: true,     
          become: true,
          playbook: 'playbook.yml',
          inventory: 'hosts.yml'
      )
    }
}

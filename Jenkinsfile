node{
  def remote = [:]
  remote.name = 'oraclevm'
  remote.host = '152.67.160.182'
  remote.user = 'opc'
  remote.password = 'Muzammil073#'
  remote.allowAnyHosts = true
    stage('checkout') {
           checkout scm
  }  
  stage('step1') {
        sshPut remote: remote, from: 'shaikimran07.sh', into: '/home/opc'
  }
  stage('step2') {
    sshCommand remote: remote, command: "shaikimran07.sh"
  }
  stage('step3') {
    sshCommand remote: remote, command: "pwd"
  }
}
  
  
  


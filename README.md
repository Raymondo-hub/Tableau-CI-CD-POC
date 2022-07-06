# Tableau-CI-CD-POC
#test for webhook
node {

  stage 'Checkout'
  git url: 'https://github.com/Raymondo-hub/Tableau-CI-CD-POC.git' , branch: 'main'

/*def remote = [:]
remote.name = 'test1'
remote.host = '10.0.0.0'
remote.user = 'rechu1'
remote.password = 'Georgio69@!'
remote.allowAnyHosts = true
  stage("copy from git to tableau-dev") {
        sshPut remote: remote, from: 'myfile.txt', into: '/folder1/'
        sshPut remote: remote, from: 'myfile.txt', into: '/folder2/'
        sshCommand remote: remote, command: 'cat myfile.txt'

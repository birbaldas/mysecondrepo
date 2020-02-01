node {
   def ws
   stage('co') {
      checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '1e36171e-a11e-41a3-bc04-41b7d502fb6a', url: 'https://github.com/birbaldas/mysecondrepo.git']]])
      ws = pwd()
      echo "fired from github..my workspace is $ws"
      
   }
   stage('Build') {
       echo "im in build stage fired from github"
     
   }
   stage('Results') {
              echo "im in result stage fired from github"

   }
}

node {
   echo 'Hello World'
   
              stage 'git checkout'
   git credentialsId: 'git', url: 'https://github.com/subbireddyg/my-app'
   
   
              stage 'Maven Pakcage'
   
   sh 'mvn clean package'
    

              body_msg = "Jeknis Job Sucess" + "$JOB_URL" + " Thanks CKP Jenkins Team " 
              stage 'Mail'
   
   mail bcc: '', body: body_msg , 
                                cc: 'subbireddy.oracle@gmail.com', from: '', replyTo: '', subject: 'Pipeline script for CKP', to: 'gajulapallisubbireddy@gmail.com'

}

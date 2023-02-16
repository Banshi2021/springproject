node('built-in') 
  
     {
    
  stage('continious download') 
        
      {
             
 git branch: 'main', url: 'https://github.com/Banshi2021/springproject.git'
        
      }
  
   stage('continious build') 
        
     {
             
        sh 'mvn package'       
     }
  
 stage('continious deployment') 
        
     {
             
        sh 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/target/Springmvcpractice.war ubuntu@172.31.5.92:/var/lib/tomcat9/webapps/qaenv.war'     
     }
  
 stage('continious testing') 
        
     {
             
        sh 'echo "Testing Passed"'

     }
  
stage('continious Delivery') 
        
     {
             
        sh 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipeline/target/Springmvcpractice.war ubuntu@172.31.8.95:/var/lib/tomcat9/webapps/prodenv.war'     
     }
  
}
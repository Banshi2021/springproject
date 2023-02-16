node('built-in') 
  
     {
    
  stage('continious download_main') 
        
      {
             
 git branch: 'main', url: 'https://github.com/Banshi2021/springproject.git'
        
      }
  
   stage('continious build_main') 
        
     {
             
        sh 'mvn package'       
     }
  
 
  
}

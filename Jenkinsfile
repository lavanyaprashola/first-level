pipeline {
agent any 
    tools {
        'maven'
         }
   stages {
     stage( "git check out "){
           steps{
                     script{
                          git branch: 'main', url: 'https://github.com/lavanyaprashola/first-level.git'
                           }
                     }
         
                  }  
                 
   stage ('Build')  {
	 steps {
      dir('src'){
            sh "mvn package"
          }
        }    
   }
  
   }
   
}

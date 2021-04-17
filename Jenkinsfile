job('dsl-job1') {
  description('Created by DSL script')
  
  
      
    scm {
        github('umeshtyagi829/java-app-maven', 'master')
    }
    
    
    steps {
                         
        maven {
        mavenInstallation('Maven')
        goals('package') 
      
        
        shell ('java -jar target/*.jar')
    }
      
 }
  
  publishers {
        archiveArtifacts('target/*.jar')
        archiveJunit('/target/surefire-reports/*.xml')
    }

}

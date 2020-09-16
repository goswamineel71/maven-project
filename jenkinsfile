pipeline {
 agent any
 Stages{
     Stage('build'){
         Steps {
             sh 'mvn clean package'
         }
         Post {
             Success {
                 Echo "Now Archiving"
                 archiveArtifacts artifacts" "**/target/*.war"
             }
         }
     }
     }
     }


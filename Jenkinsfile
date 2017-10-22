pipeline {
        agent any
        
        stages {
                stage ('Compile Stage') {
                        steps  {
                                withMaven(maven : 'apache-maven-3.5.0'){
                                         sh 'maven test'               
                                }
                          }
                 } 
                  
                stage ('Testing Stage') {
                        steps  {
                                withMaven(maven : 'apache-maven-3.5.0'){
                                         sh 'maven clean compile'
                                }
                          }
                 }
                 stage ('Installing Stage') {
                        steps  {
                                withMaven(maven : 'apache-maven-3.5.0'){
                                         sh 'maven install'
                                 }
                          }
                   
                   ]
                stage ('Deployment Stage') {
                        steps  {
                                withMaven(maven : 'apache-maven-3.5.0'){
                                         sh 'maven deploye'
                                }
                          }
                }                
        }                                     
              

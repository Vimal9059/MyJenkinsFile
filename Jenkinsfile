pipeline {
  agent any
  environment {
     PATH ="/opt/maven/bin:$PATH"
           }
  stages {
    stage ('Git Clone') {
       steps {
          git url:'https://github.com/Vimal9059/war-web-project.git',branch:'master'
       }
     }
    stage ('Build') {
       steps {
          sh " mvn clean package "
       }
     }   
   }
 }

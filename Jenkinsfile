pipeline {
    agent any  
        stages {
          stage('continuos download') {
              steps {
            git 'https://github.com/Premvikash/java-maven-sample-war.git'
            }
        }
               stage('continuos build') {
                   steps {
                  sh 'mvn install'
            }
        }
                  stage('continuos deployment') {
                      steps {
                    sh 'cp target/Example-0.0.1-SNAPSHOT.war /var/lib/apache-tomcat-9.0.56/webapps'
            }
        }
    }
 }





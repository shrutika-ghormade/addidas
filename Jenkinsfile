pipeline {
        agent any

        stages {
           stage('Checkout') {
               steps {
                      checkout scm
                     }}
               stage('Build') {
                  steps {
                         sh '/home/shrutika/Documents/Devops-software/apache-maven-3.9.1/bin/mvn install'
                        }}
               stage('Deployment'){
                       withCredentials([string(credentialsId: 'shrutikaghormade', variable: 'jumbo')]) 
                       sh 'docker login -u shrutikaghormade -p${docker jumbo}
}
                  steps {
                         sh 'cp target/addidas.war /home/shrutika/Documents/Devops-software/apache-tomcat-9.0.73/webapps
         }
}}}


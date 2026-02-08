pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
               sh "/opt/apache-maven/bin/mvn clean -o"
             }
         }
        stage('Test') {
            steps {
               sh "/opt/apache-maven/bin/mvn test -o"
             }
         }
        stage('Deploy') {
            steps {
               sh "/opt/apache-maven/bin/mvn package -o"
            }
         }
     }
}

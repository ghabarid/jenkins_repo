pipeline {
  agent any
  stages{
      stage('Clean stage'){
        steps {
          withMaven(maven: "Maven 3"){
            sh 'mvn clean'
          }

        }
      }

      stage('Compile stage'){
              steps {
                withMaven(maven: "Maven 3"){
                  sh 'mvn compile'
                }

              }
      }

      stage('Package stage'){
              steps {
                withMaven(maven: "Maven 3"){
                  sh 'mvn package'
                }

              }
            }
  }

}


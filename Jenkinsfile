node {
  stage ('Build Jar  ') {
    git url: 'https://github.com/gansky770/ciexercise.git'
    withMaven(maven: 'Maven-3.6.3', mavenSettingsConfig: 'bed37eaa-e653-4633-b495-f16d9d3d3b93') {
      sh "mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -"
    } // withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe reports and FindBugs reports
  }

 // stage('SonarQube analysis') {
   // withSonarQubeEnv(credentialsId: 'SonarCloud', installationName: 'SonarCloud') { // You can override the credential to be used
      //sh 'mvn org.sonarsource.scanner.maven:sonar-maven-plugin:3.7.0.1746:sonar'
    //}
 // }

  stage ('SonarQube analysis') {
      
  }
}

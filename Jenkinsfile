node {
  stage ('Build Jar  ') {
    git url: 'https://github.com/gansky770/ciexercise.git'
    withMaven(maven: 'Maven-3.6.3', mavenSettingsConfig: '32acdde9-f4d2-4c43-b0e8-dbcb51554d0c') {
      sh "mvn clean verify sonar:sonar -Dsonar.login=myAuthenticationToken"
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

pipeline {

  agent any
  stages {
    stage('Build') {
      steps {
            echo "build success"
      }
    }

    stage('Test') {
      steps {
          echo "mvn test starts"
      }
    }

     stage('Deploy Development') {
      steps {
            bat 'mvn clean package deploy -DmuleVersion=4.4.0 -Dusername=spandan_maity1 -Dpassword=SampleNewPass221 -DapplicationName=cicdsample -Denvironment=Sandbox -Dworkers=1 -DworkerType=Micro -DmuleDeploy'
      }
    }
}
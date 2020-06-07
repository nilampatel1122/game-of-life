
pipeline{
    agent any
    tools{
          maven 'mvn'
          jdk 'jdk'
         }
stages{
    stage("sync")

    {
        steps
        {
            git 'https://github.com/nilampatel1122/game-of-life.git'
        }
   }
    stage("buid"){
        steps
        {
            sh "mvn clean package"
        }
                   }
        stage("test")
        {
           steps{
              junit '**/target/surefire-reports/TEST-*.xml'
            }
        }
        stage("archive"){
            steps{
                archive 'target/*'
            }
        }
}        
    }


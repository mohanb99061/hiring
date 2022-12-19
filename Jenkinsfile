pipeline{
    agent any
    stages{
        
        stage('Maven Build'){
            when {
                branch 'develop'
            }
        steps{
            sh "mvn clean package"
        }
    }
    stage('Tomcat Deploy - Dev'){
        when{
            branch 'develop'
        }
        steps{
            echo "Deplying to dev"
} 
        }
        
        stage('Tomcat Deploy - Prod'){
        when{
            branch 'develop'
        }
        steps{
            echo "Deplying to production"

        }
    }
  }
}

pipeline{
    agent any
    
    stages{
    
        stage('Build'){
                 when{
                 BuildingTag()
                 }
        
                steps{
                    
                    echo "This Pipeline is working"
                }
            }
            stage('Dev'){
                 when{
                 DevTag()
                 }
        
                steps{
                    
                    echo "This Pipeline is working"
                }
            }
        }
}

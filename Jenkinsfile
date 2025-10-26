pipeline{
     agent any
   
    stages{
        stage("Restore some Dependencies"){
            steps{
                bat 'dotnet restore'
            }
          
        }
        stage("Build the applcication"){
            steps{
                bat 'dotnet build --no-restore'
            }
          
        }
         stage("Run the tests"){
            steps{
               bat 'dotnet test --no-build --verbosity normal'
            }
          
        }
    }
    
}

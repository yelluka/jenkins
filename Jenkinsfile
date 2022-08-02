pipeline{
    agent none
        stages
            stage ('Build') {
                steps{
                    echo 'hello woreld!!'
                }    
            }
            stage ('Deploy') {
                When{
                    before input true
                    branch 'production'
                    
                }
                input {
                    message "deploy to production"
                    id "simpule - input"
                }
                steps{
                echo 'deploying'
            }
        }
    }     

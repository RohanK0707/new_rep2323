pipeline {
    
    agent any
    
    stages {
        
        stage ('stage-1') {
            
            steps {
                
                
                sh "sudo yum install httpd -y"
                sh "sudo service httpd start"
                
               
                
            
            }
        }
        
        stage ('stage-2') {
            
            steps {
                
                
                
                sh "sudo echo hello > /var/www/html/index.html "
                sh "chmod 777 /var/www/html/index.html"
            }
        
        
    }
}}

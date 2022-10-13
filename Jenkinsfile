pipeline 
{
    agent
	{
		label 'QA'
	}
	stages 
	{
		stage ('HTTP Service Install on Jenkis Master')
		{
			steps 
			{
				echo "Installing HTTPD Service"
				sh "sudo yum update -y"
				sh "sudo yum install httpd -y"
				sh "sudo chkconfig httpd on"
				sh "sudo service httpd start"
				sh "sudo echo My First Page >> /var/www/html/index.html"
				sh "sudo chmod -R 777 /var/www/html/index.html"
			
			}
		}
    }
}

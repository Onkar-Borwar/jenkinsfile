pipeline
{
   agent 
    {
          label('slave1')
    }

stages

    {  
        stage ('Install Apache')
               {
                  steps
                  {
                     sh "sudo yum remove httpd -y"
                 sh "sudo yum install httpd -y"
                  }
               }
       stage ('Start Apache')
                  {
                  steps
                  {
                     sh "sudo service httpd start"
                  }
                  }
       stage ('Deploye index')
                  {
                  steps         
                     {
                        sh "sudo cp -r index.html /var/www/html"
                 sh "sudo chmod -R 777 /var/www/html/index.html"
                  }
               }
    }
}


pipeline
{
   agent 
    {
          label('slave2')
    }

stages

    {  
        stage ('Install Apache')
               {
                  step
                  {
                 sh "sudo yum install httpd -y"
                  }
               }
       stage ('Start Apache')
                  {
                  step
                  {
                     sh "sudo service httpd start"
                  }
                  }
       stage ('Deploye index')
                  {
                  step         
                     {
                        sh "sudo cp -r index.html /var/www/html"
                 sh "sudo chmod -R 777 /var/www/html/index.html"
                  }
               }
    }
}


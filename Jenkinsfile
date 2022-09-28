


pipeline
{
   agent 
    {
          label('slave2')
    }

stages

    {  
        stage ('Insatall Apache')
               {
                 sh "yum install httpd -y"
                 sh "service httpd start"
                 sh "cp -r index.html /var/www/html"
                 sh "chmod -R 777 /var/www/html/index.html"

               }
    }
}


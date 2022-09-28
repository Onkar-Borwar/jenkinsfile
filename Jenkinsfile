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
                 sh "sudo yum install httpd -y"
                  sh "sudo sleep 20"
                 sh "sudo service httpd start"
                 sh "sudo cp -r index.html /var/www/html"
                 sh "sudo chmod -R 777 /var/www/html/index.html"

               }
    }
}


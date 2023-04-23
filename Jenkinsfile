pipeline{
agent any
stages{
 stage('copy-dev'){
 steps{
     sh 'cp -r dev.html /var/www/html'
      }
	} 
 stage('copy-qa'){
 steps{
     sh 'cp -r qa.html /var/www/html'
      }
	}  
 stage('copy-uat'){
 steps{
     sh 'cp -r uat.html /var/www/html'
      }
	}  
 stage('restart-apache'){
 steps{
     sh 'sudo service httpd restart'
      }
	}  
 }
}

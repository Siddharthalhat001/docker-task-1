node
{
   stage('SCM Checkout')
   {
       git branch: 'main', credentialsId: 'git-cred', url: 'https://github.com/Siddharthalhat001/docker-task-1.git'
   }
   
   stage('Mvn Package'){
    
     sh "mvn clean package"
     
   }
   stage('Build Docker Image')
   {
       sh "docker build -t siddharthalhat001/job-1-image:1.0 . "
   }
    stage('Push Docker Image')
   {
       sh "docker push siddharthalhat001/job-1-image:1.0  "
   }}


node {
   def mvnHome
   stage('Preparation') { 
      git 'https://github.com/ppr83/course.git'
      mvnHome = tool 'maven_home'
   }
   stage('Build') {
      // Run the maven build
         sh "'${mvnHome}/bin/mvn'  clean package"
   }
   stage('Results') {
    echo "successful"
   }
}
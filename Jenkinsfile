pipeline{
agentany

stages{
stage('scm checkout'){
steps{
sh "git clone https://github.com/mano8888/aws-6.git"
}
}
stage('build'){
step{
sh "mvn clean -f aws-6"
}
}
stage('test'){
steps{
sh "mvn test -f aws-6"
}
}
stage('mvn deploy'){
steps{
sh "mvn packages -f aws-6"
}
}
}
}


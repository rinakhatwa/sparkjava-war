pipeline 
{
    agent any
	environment 
	{
		PATH="/opt/maven/bin:$PATH"
	}
    stages 
    {
        stage('git clone') 
        {
            steps
            {
               git url : 'https://github.com/rinakhatwa/sparkjava-war.git', branch: 'master'
            }
        }
        stage('Build')
        {
            steps
            {
               sh 'mvn clean install'
            }
        }
 
    }
}

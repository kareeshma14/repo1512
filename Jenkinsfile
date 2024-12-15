pipeline {
    agent {
        node{
            label 'maven'
        }
    }
    environment{
        PATH = "/opt/apache-maven-3.9.9/bin:$PATH"
    }

    stages {
        stage("build"){
            steps{
                sh 'mvn deploy -DaltDeploymentRepository=your-repo-id::default::http://your-repo-url
'
            }
        }
    }
}
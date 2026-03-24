pipeline {
    agent { labels 'docker' }
    triggers {
        pollSCM('H/2 * * * *')   // every 2 minutes
    }

    stages {
        stage('Clone Repository') {
            steps {
git branch: 'main',
                    url: 'git@github.com:ManjuSKM/devOpsonAWSTraining.git',
                    credentialsId: 'github-creds'                
            }
        }

    stage('Check the docker cli') {
      steps {
        sh "docker --version"
        sh "docker ps -a"
      }
    }
        stage('Docker-Build') {
            steps {
                echo "Docker-Build step here..."
                sh "docker build . -t pythonapp:v1"
            }
        }

        stage('DockerContainer Creation') {
            steps {
                echo "Running Docker compose here..."
                sh "docker compose up -d"
            }
        }

    }
}

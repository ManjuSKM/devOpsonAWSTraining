pipeline {
    agent { labels 'docker' }
    triggers {
        pollSCM('H/2 * * * *')   // every 2 minutes
    }

    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/your-username/your-repo.git',
                    branch: 'main'
            }
        }

        stage('Build') {
            steps {
                echo "Build step here..."
            }
        }

        stage('Test') {
            steps {
                echo "Test step here..."
            }
        }
    }
}pipeline {
    agent { label 'docker' }
    triggers {
        pollSCM('H/2 * * * *')   // every 2 minutes
    }

    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/your-username/your-repo.git',
                    branch: 'main'
            }
        }

        stage('Build') {
            steps {
                echo "Build step here..."
            }
        }

        stage('Test') {
            steps {
                echo "Test step here..."
            }
        }
    }
}pipeline {
    agent { label 'docker' }
    triggers {
        pollSCM('H/2 * * * *')   // every 2 minutes
    }

    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/your-username/your-repo.git',
                    branch: 'main'
            }
        }

        stage('Build') {
            steps {
                echo "Build step here..."
            }
        }

        stage('Test') {
            steps {
                echo "Test step here..."
            }
        }
    }
}

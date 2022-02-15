pipeline {
    stages {
        stage("Build") {
            steps {
                echo "Build"
            }
        }
        stage("Test") {
            steps {
                echo "Test"
            }
        }
        stage("Scan") {
            steps {
                echo "Scan"
            }
        }
        stage("Deploy") {
            when {
                branch "main"
            }
            steps {
                echo "Deploy
            }
        }
        stage("Release") {
            when {
                buildingTag()
            }
            steps {
                echo "Archive"
            }
        }
    }
}

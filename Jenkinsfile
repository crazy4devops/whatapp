pipeline{
    agent any
    stages{
        stage("Checkout"){
            steps{
                git url: "https://github.com/crazy4devops/whatsapp.git", branch: "dev"
            }
        }
        stage("Build for linux"){
            agent { label "linux-agent" }
            steps{
              echo "This build is for Linux Builds"
            }
        }
        stage("Build for windows"){
            agent { label "windows-agent" }
            steps{
              echo "This build is for Windows Builds"
            }
        }
        stage("Build for macos"){
            agent { label "macos-agent" }
            steps{
               echo "This build is for Macos Builds"
            }
        }
    }
}
# Update package information and install OpenJDK 11
sudo apt update
sudo apt install openjdk-11-jdk

# Add Jenkins repository keyring and repository
curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo gpg --dearmor -o /usr/share/keyrings/jenkins-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/jenkins-archive-keyring.gpg] https://pkg.jenkins.io/debian-stable binary/" | sudo tee /etc/apt/sources.list.d/jenkins.list

# Update package information again and install Jenkins
sudo apt update
sudo apt install jenkins

# Start and enable Jenkins service
sudo systemctl start jenkins
sudo systemctl enable jenkins
sudo systemctl status jenkins


# Install Docker
sudo apt install docker.io

# Create a Jenkinsfile (assuming you have a specific script in mind)
# You can create the Jenkinsfile using any text editor you prefer, such as "nano" or "vim".
# For demonstration purposes, let's create a simple Jenkinsfile using "echo".
echo 'pipeline {
    agent any
    stages {
        stage("Hello") {
            steps {
                echo "Hello, Jenkins!"
            }
        }
    }
}' > Jenkinsfile

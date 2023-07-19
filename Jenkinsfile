pipeline {
    agent any
    
    stages {
        stage('SSH Login') {
            steps {
                script {
                    def remoteServer = '192.168.1.76'
                    def remoteUser = 'root'
                    def remotePassword = '1'
                    
                    // SSH login and execute commands
                    sshCommand remote: remoteServer, user: remoteUser, password: remotePassword, command: '''
                        echo "Hello, remote server!" > /root/asimJenkins
                        # Add more commands here
                    '''
                }
            }
        }
        
        // Add more stages as needed
        
    }
}

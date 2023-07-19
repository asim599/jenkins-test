pipeline {
    agent any
    
    stages {
        stage('SSH Login') {
            steps {
                script {
                    def remoteServer = '103.83.89.237'
                    def remotePort = 8010
                    def remoteUser = 'root'
                    def remotePassword = '1'
                    
                    // SSH login and execute commands
                    sshCommand remote: remoteServer, port: remotePort, user: remoteUser, password: remotePassword, command: '''
                        echo "Hello, remote server!" > /root/asimJenkins
                        # Add more commands here
                    '''
                }
            }
        }
        
        // Add more stages as needed
        
    }
}

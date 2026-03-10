​pipeline {
    agent any
    stages {
        stage('Publish') {
            steps {
                publishHTML([
                    allowmissing: true,
                    alwaysLinktoLastBuild: false,
                    keepAll: false,
                    reportDir: '.',
                    reportFiles: 'file.html',
                    reportName: 'MY HTML PIPE PAGE'
                ])
            }
        }
    }
}

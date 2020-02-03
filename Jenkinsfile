pipeline {
    agent any

    stages {
        stage('find zip length') {
            
                def script ='du -k my_zip_file.zip | cut -f1'
				size = sh(script: script, returnStdout: true)
				print(size)
            
        }
    }
}
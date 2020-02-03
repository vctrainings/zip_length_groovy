node{
        
		stage('Clone sources') {
			git url: 'https://github.com/vctrainings/zip_length_groovy.git'
		}
		stage('find zip length') {
            
                def script ='du -k my_zip_file.zip | cut -f1'
				size = sh(script: script, returnStdout: true)
				if(size<100){
					print("File is less than 100kb, Hence good to upload")
				}
            
        }
    }

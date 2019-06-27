
node {
	stage 'Checkout'
	
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/soorya79/jenkinsFile_task.git']]])
	 
	stage 'Syntax Check'
	
	sh 'ansible-playbook --syntax-check ./task1.yml' 
	
	stage 'Check for playbook'
	
	if (fileExists('task1.yml')) {
    	echo 'Playbook exists'
	} 
	else 
	{
    	echo 'Playbook doesnot exists'
	}
	
	stage 'Execute playbook'
	sh 'ansible-playbook task1.yml'
	
	
}

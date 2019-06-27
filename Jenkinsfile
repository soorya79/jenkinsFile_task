
node {
	
	stage 'Syntax Check'
	
	sh 'ansible-playbook --syntax-check ./task1.yml' 
	
	stage 'Check for playbook'
	
	if (fileExists('file')) {
    	echo 'Yes'
	} 
	else 
	{
    	echo 'No'
	}
	
	
}

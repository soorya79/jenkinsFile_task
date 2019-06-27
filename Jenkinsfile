node {
	stage 'Checkout'
	
        checkout scm
	
	stage 'Syntax Check'
	
	sh 'ansible-playbook --syntax-check ./task1.yml' 
	
	
	
}

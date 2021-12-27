node('notnetcore'){
	stage('SCM'){
		checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/marsshan2018']]])
	}
	stage('Build'){
		sh 'dotnet build HelloWorld'
	}
	stage('Test'){
		echo 'Execute unit tests here'
	}
	stage('Package'){
		echo 'Zip it up'
	}
	stage('Deploy'){
		echo 'Push to deployment'
	}
}

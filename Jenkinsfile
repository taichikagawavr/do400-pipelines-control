node('nodejs') {

	stage('Checkout') {
		git branch: 'main',
			url: 'https://github.com/taichikagawavr/do400-pipelines-cntrol'
	}

	stage('Backend Tests') {

		sh 'node ./backend/test.js'

	}

	stage('Frontend Tests') {

		sh 'node ./frontend/test.js'

	}
}

pipeline{
	agent any
	stages{
		stage('deleting')
                {
                        steps{
                                sh 'rm -r *'
								sh 'rm -r ../../../../www/html/*'
								
								

                        }
                }
		
		stage('cloning from SCM')
                {
                        steps{
                                sh 'git clone https://gitlab.com/kartikbalekaru/website.git -b master'
								sh 'pwd'
								// sh 'cd website'
								// sh 'rm -r *'
								// sh 'mv * ..'
								// sh 'pwd'

                        }
                }
				stage('copy to html')
                {
                        steps{
                                sh 'mv website/* ../../../../www/html'
								// sh 'pwd'
								// sh 'cd website'
								// sh 'rm -r *'
								// sh 'mv * ..'
								// sh 'pwd'

                        }
                }
		// stage('super user')
		// 		{
		// 				steps{
		// 						sh 'sudo su -s'

		// 				}
		// 		}
		// stage('come back')
		// 		{
		// 				steps{
		// 						sh 'cd ../..'

		// 				}
		// 		}
		// stage('apache2')
		// 		{
		// 				steps{
		// 						sh 'apt-get install apache2 -y'

		// 				}
		// 		}
		// stage('move to html')
		// 		{
		// 				steps{
		// 						sh 'cd var/www/html'

		// 				}
		// 		}
		// stage('cloning')
		// 		{
		// 				steps{
		// 						sh 'git clone https://gitlab.com/kartikbalekaru/website.git -b master'

		// 				}
		// 		}
        // stage('deleting index.html')
		// 		{
		// 				steps{
		// 						sh 'rm index.html'
		// 						sh 'cd website'

		// 				}
		// 		}
        // stage('moving folder')
		// 		{
		// 				steps{
		// 						sh 'mv * ..'

		// 				}
		// 		}

	}
}
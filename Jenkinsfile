node{
try
{
stage('Checkout')
    {
git 'https://github.com/majdas007/Blog-Post'
    }
stage('INSTALL dependencies')
    {
sh "npm install"
    }
stage('RUN Unit Tests'
    {
sh "npm run test:unit"
    }
} catch (err) 
      {
    currentBuild.result = 'FAILURE'
      }
}

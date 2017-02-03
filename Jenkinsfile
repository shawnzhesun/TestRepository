node('assistant') {
   properties([pipelineTriggers([[$class: 'GitHubPushTrigger']])])
   checkout scm
   sh """
	pwd
        curl -H "Accept: application/json" -H "Content-Type: application/json" -H "Authorization: Basic QkE6QkE=" -X GET https://c3iotadmin.c3-e.com/api/1/reference/prod/User?action=fetch
   """
   println env.BRANCH_NAME
   println scm.branches[0].name
    
}
  
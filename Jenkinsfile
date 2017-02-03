node('assistant') {

   sh """
	pwd
        curl -H "Accept: application/json" -H "Content-Type: application/json" -X POST https://BA:BA@c3iotadmin.c3-e.com/api/1/reference/prod/Cluster?action=hosts
   """
   println env.BRANCH_NAME
   println scm.branches[0].name
   
}

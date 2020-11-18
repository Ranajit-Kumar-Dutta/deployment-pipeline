# deployment-pipeline

1) The build triggers as soon as anyone in the dev team merges code to main branch.
2) The trigger builds all the 3 projects - Web, API and test, Assuming there are different projects for Web, API and test in the same solution.
   The build should is unsuccessful if any test fails.
3) The deployment of code and artifacts is automated to Dev environment provided build is successful.
4) Upon successful deployment to the Dev environment, deployment is promoted to QA and Prod through automated process.
5) Environments for QA is QA_app and for prod is prod_app. I have configured Approvals and Checks in these environments in Azure DevOps.

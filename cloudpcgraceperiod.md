Go to https://aka.ms/ge


Log in with Admin account.
Consent to permission-> Agreement-> Consent the permission.
Modify permission -> Consent the permission
[List cloudPCs - Microsoft Graph v1.0 | Microsoft Learn](https://learn.microsoft.com/en-us/graph/api/virtualendpoint-list-cloudpcs?view=graph-rest-1.0&tabs=http) : List you All cloud pc
GET https://graph.microsoft.com/v1.0/deviceManagement/virtualEndpoint/cloudPCs
Run the Query -> You will see all your CPC and its grace period end data/time
Copy the ID of affected CPC and paste it somewhere else.
[cloudPC: endGracePeriod - Microsoft Graph v1.0 | Microsoft Learn](https://learn.microsoft.com/en-us/graph/api/cloudpc-endgraceperiod?view=graph-rest-1.0&tabs=http) : End grace period.
POST https://graph.microsoft.com/v1.0/deviceManagement/virtualEndpoint/cloudPCs/4b18de4b-ab05-4059-8c61-0323a7df4ced/endGracePeriod
Paste your Affected CPC ID in place of highlighted ID
Run the query -> Grace period ended
Now List your All cloud pc again
GET https://graph.microsoft.com/v1.0/deviceManagement/virtualEndpoint/cloudPCs
Run the Query -> You will see all your CPC and the grace period of affected CPC is null.
You can now assign license to different user.
Graph Explorer | Try Microsoft Graph APIs - Microsoft Graph
Try the Graph Explorer developer tool to learn about Microsoft Graph APIs. Includes code snippets, Microsoft Graph Toolkit, and Adaptive Cards integration.

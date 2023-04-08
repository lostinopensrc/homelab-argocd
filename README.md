Add the remote Github repository :

$ git remote add origin "<HTTPS_URL_OF_GITHUB_REPO>"

Add below git configs to be used for commits on your GIthub repo :

$ git config --local user.name <GITHUB_USERNAME>

$ git config --local user.email  <GITHUB_EMAILID>

Add below git config so that you can get access to your Github repository :

git config --global credential.username <GITHUB_USERNAME>


POST ArgoCD installtion : 

Get the below initial password to intially login with usernam:admin . Remember to change admin password from GUI immediately: 

$ kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d

![[Pasted image 20230408120205.png]]
### How to add the helm repo to install my charts


## Package chart, index and push to git

`helm package nginx`

`helm repo index github-helm/ --url https://sandeeplamb.github.io/helm-kubernetes/`

`git commit -a -m "change index"`

`git push origin`

## Add the Repo

`helm repo add github-helm  https://sandeeplamb.github.io/helm-kubernetes/.`

`helm repo list`

## Install the helm chart

`helm install github-helm/nginx --name=nginx-my-repo --dry-run --debug`

`helm install github-helm/nginx --name=nginx-my-repo --debug`
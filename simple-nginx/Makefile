deploy-prod:
	kubectl config use-context arn:aws:eks:sa-east-1:250135344706:cluster/confia-prod
	helm upgrade -i --create-namespace -n simple-nginx-dev simple-nginx-dev . -f values.yaml

remove-prod:
	kubectl config use-context arn:aws:eks:sa-east-1:250135344706:cluster/confia-prod
	helm uninstall -n simple-nginx-dev simple-nginx-dev

```bash 
# login ecr 
aws ecr get-login-password --region ap-southeast-2 --profile default | docker login --username AWS --password-stdin 655082996631.dkr.ecr.ap-southeast-2.amazonaws.com

# build and push 
image="655082996631.dkr.ecr.ap-southeast-2.amazonaws.com/sock-shop/carts:latest"
docker build -t $image . && docker push $image
```

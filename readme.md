# get into container shell
docker exec -it flask-hello_flask_1 bash

# run python script in container
docker exec -it flask-hello_flask_1 python train_model.py

# curl post request json
curl --header "Content-Type: application/json" \
  --request POST \
  --data '{"flower":"1,2,3,7"}' \
  http://localhost:5000/iris_post

  # how to create an instance at aws ec2
  https://aws.amazon.com/getting-started/tutorials/launch-a-virtual-machine/

  # ssh to aws ec2
ssh -i ~/.ssh/MyKeyPair.pem ec2-user@18.220.35.31
# Public DNS: ec2-18-220-35-31.us-east-2.compute.amazonaws.com
ssh -i ~/.ssh/MyKeyPair.pem ec2-user@ec2-18-220-35-31.us-east-2.compute.amazonaws.com

# check what's taking up port
netstat -vanp tcp | grep 5001

sudo lsof -i :5001

# start container
docker-compose up

docker-compose up --build #and build

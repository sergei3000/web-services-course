# get into container shell
docker exec -it flask-hello_flask_1 bash

# run python script in container
docker exec -it flask-hello_flask_1 python train_model.py

# curl post request json
curl --header "Content-Type: application/json" \
  --request POST \
  --data '{"flower":"1,2,3,7"}' \
  http://localhost:5000/iris_post
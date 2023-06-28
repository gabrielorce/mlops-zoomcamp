
## My Homework

# converting the notebook to script:
```
jupyter nbconvert --to script starter.ipynb
```

# pipenv creation was installed and then activated with:
```
pipenv install scikit-learn==1.2.2 pandas  --python=3.9
pipenv shell
```

# Docker creation and execution commands. Notice the inpu variables (year=2022, month=4)
```
docker build -t prediction-service:v1 .
docker run -it --rm prediction-service:v1 2022 4
```

NOTE: Docker takes a while to actually show the output, for some reason
NOTE2: I had to add the following line to /etc/default/docker in my WSL because pipenv would not download 
```
DOCKER_OPTS="--dns 8.8.8.8 --dns 8.8.4.4"
```

 
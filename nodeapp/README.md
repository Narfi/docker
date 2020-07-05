# Example usage:
## Build
    docker build -t nodeapp:latest .
## Run
    docker run \
	-d \
	--restart=always \
	--name=helloworld \
	-v /home/user/workspace/helloworld/:/src/ \
	-p 3000:3000 \
	nodeapp \
	sh -c 'npm install && npm start'
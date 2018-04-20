

1. creating the docker images for custom sw
	build*Image scripts are doing the job

2. starting the docker images
sudo docker run -d -p 6379:6379 redis
sudo docker run --network host -p 8090:8090 -d ibisdev/node-webfeed
sudo docker run --network host -p 8080:8080 -d ibisdev/node-vehicle_handler


3. Checking the logs:
	docker log <idOfTheContainer>

4. checking the filesystem:
	docker run -t -i <idOfTheContainer> /bin/bash


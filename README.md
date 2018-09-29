      $ cd ccminer-in-docker
      $ docker build -t ccminer/docker .
      $ nvidia-docker run -d \
      --name=ccminer \
      -e ALGO=<algorithm> \
      -e MINING_POOL=<MINING_POOL_WITH_PORT> \
      -e USER_NAME=<USERNAME/WORKERNAME> \
      -e PASSWORD=<PASSWORD> \
      -v /etc/localtime:/etc/localtime:ro \
      ccminer/docker 
      
Logs

      docker logs -f ccminer

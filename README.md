# acsn-windows-docker-image
Used for A Cloud Security Ninja LLC Windows Docker Image


# How to Test Image Locally

Run the following Commands to create a windows GUI within Docker Desktop and your browser using QEMU - noVNC

1. Run this command below
```bash
docker system prune --all --force
```

2. Run this command below
```bash
docker compose up -d
```

3.  Once it says started then you can go into Docker Desktop and see that the container is downloading Windows 10 from Microsoft. You should see a percentage and it may take up to 10 minutes to download. It will make a local windows folder that holds the ISO and information tied to the container. Please keep this while you are using it ,but do not upload to the github repos as its too large. I have this ignored already using .gitignore method. If you delete though you will need to re configure everything. 

4. Once the Docker Container is downloaded. The next step is to get into the Windows System in your browser and it should show the URL in docker desktop in the container itself. It should be something similar to http://127.0.0.1:8006.

5. At this time your host system may be a bit slow but the windows installation will be automatic and shouldn't take more than 30 minutes. Once this is completed the performance is improved!

6. Once installed you can stop and start the windows machine from within the Docker Desktop Containers Section. 

7. At this point as long as you have the /windows folder locally it will keep your windows docker container information and can be used later.



## Credit 

- https://github.com/dockur/windows
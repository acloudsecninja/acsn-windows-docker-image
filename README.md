# acsn-windows-docker-image
Used for A Cloud Security Ninja LLC Windows Docker Image


# - How to Test Image

- Run the following Commands

1. docker system prune --all --force

2. You need to go into the wslconfig settings to change you default settings to increase the disk size. https://learn.microsoft.com/en-us/windows/wsl/wsl-config#configure-global-options-with-wslconfig

3. docker run -it --rm --name windows -e "VERSION=11" -p 8006:8006 --device=/dev/kvm --device=/dev/net/tun --cap-add NET_ADMIN -v "${PWD:-.}/windows:/storage" --stop-timeout 120 docker.io/dockurr/windows

4. 



## Credit 

- https://github.com/dockur/windows
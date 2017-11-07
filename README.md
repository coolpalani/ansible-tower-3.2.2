# Ansible Tower Docker Image

## How to run this image

### 1. Build or pull the image

```docker build -t coolpalani/ansibletower .```

or 

```docker pull coolpalani/ansibletower ```

### 2. Get a license

Reachout RedHat team to get a licence file.
http://www.ansible.com/license

### 3. Run the image

```
docker run -it \
	-p 80:80 -p 443:443 \
	-v /pathofthedirectory/license.txt:/etc/tower/license \
	--name tower \
	--privileged \
	coolpalani/ansibletower
```

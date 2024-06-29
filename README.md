# Linux_command

Stop and remove all dockers
```bash
sudo docker stop $(sudo docker ps -q);sudo docker rm $(sudo docker ps --filter status=exited -q)
```

Delete dictionary
```bash
rm -r dic_name
```

Latest FEniCS in Docker (Linux/MacOS)
```bash
docker run -ti -p 127.0.0.1:8000:8000 -v $(pwd):/home/fenics/shared -w /home/fenics/shared quay.io/fenicsproject/stable:current
```

Latest FEniCS in Docker (Windows)
```bash
docker run -ti -p 127.0.0.1:8000:8000 -v %cd%:/home/fenics/shared -w /home/fenics/shared quay.io/fenicsproject/stable:current
```

Gmsh install
```bash
sudo apt-get update;sudo apt-get install libglu1;sudo apt-get install libxcursor1;sudo apt-get install libxinerama1;pip3 install gmsh-sdk --user;pip3 install gmsh --user;pip3 install lxml --user;
```

Just for my education of GLFW and OpenGL

***********Prepare for build*************
Ubuntu 22.04:
https://medium.com/geekculture/a-beginners-guide-to-setup-opengl-in-linux-debian-2bfe02ccd1e
-   sudo apt-get install mesa-utils libglu1-mesa-dev freeglut3-dev mesa-common-dev cmake pkg-config libglew-dev libglfw3-dev libglm-dev libao-dev libmpg123-dev -y

-   git clone https://github.com/glfw/glfw.git
cmake .
make 
sudo make install

glad
https://glad.dav1d.de/
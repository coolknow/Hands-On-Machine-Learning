# Before ML
***To do a good job, an artisan needs the best tools.*** Before embarking on a machine learning project, we first need to set up a suitable development environment. In this section, I will describe the preparations that are made before a machine learning project is carried out. For example, acquiring a GPU, installing CUDA, configuring Miniconda and other tasks. Let's get started!

### GPU
You may ask me if I really need a GPU to train machine learning? The answer is **YES**.This graph shows how fast GPU is compared with CPU.

![avatar](/GPU-SSL-Jupyter/gpu.png)

As you can see that GPU is 82x faster than CPU. So, it is way faster to train a modal with GPU compared with CPU. There are lots of GPU provider you can rend from. So, i am gonna leave it here and you can choose whatever GPU provider you like. 

### SSH Remote Connection
After you having a GPU(ECS), you may consider how to use it in a proper way. Here is my suggestion. If you are using Mac, for example, try `ssh [name]@[public IP]` in your terminal. and than you will be ased to enter the password of your ecs. Do it and you will finish the connection part. If you encounter any question here, search 'linux ssh usage' at google. 

### Linux
You are still facing black terminal GUI, right? Don't worry, Let's set up the environment first and than I will give you a powerful pick. Alright, let me introduction a few linux terms so that you can play with it in the terminal. 
- `sudo` gives you the right as a root user.
- `apt-get` is a package management tool in Ubuntu that can be used to install and uninstall packages, to upgrade packages, and to upgrade the system to a new version.
- `wget` is a tool for downloading files, which is used at the command line. It is an essential tool for Linux users, we often have to download some software or restore backups from a remote server to the local server.
# Modified Docker Image of NVIDIA DIGITS

Show Caffe training accuracy by modified prototxt.

![caffe-training-accuracy](https://github.com/SoraLab/digits-docker/blob/master/img/caffe-training-accuracy.png)

# Docker Image

    $ docker pull nvidia/digits:6.0
    $ docker pull soralab/digits

or

    $ docker pull nvidia/digits:6.0
    $ git clone https://github.com/SoraLab/digits-docker
    $ cd digits-docker/6.0
    $ docker build -t soralab/digits .

# Docker Container

    $ nvidia-docker run --name digits6 -d \
      -p 5000:5000 \
      -p 6006:6006 \
      -v /path/to/digits-jobs:/jobs \
      -v /path/to/data:/data \
      soralab/digits

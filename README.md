# smartaudio-docker

Container docker to be able to play sound, functional with: https://www.waveshare.com/wiki/WM8960_Audio_HAT

## Balenablocks-audio
- this docker image is based from: https://github.com/balenablocks/audio
- You can modify the dockerfile to your system architecture, referring to: https://www.balena.io/docs/reference/base-images/base-images-ref/

## How to use
- ```git clone https://github.com/MiroYld/smartaudio-docker.git```
- ``` cd /smartaudio-docker.git```
- ```docker login``` you must be connected to docker hub to be able to build the image
- ```sudo docker build -f Dockerfile -t audio .```
- ```sudo docker run --privileged -it audio bash``` 

## Sox
- sox package: https://doc.ubuntu-fr.org/sox is already installed, you can use it to play wav file

### example
- Run your container in interactive mode
- ```play /test/test.wav```

## Thanks to the balena team for helping me to achieve this

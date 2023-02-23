FROM ubuntu:20.04

RUN apt-get update 
RUN apt-get upgrade -y

# Install gstreamer and opencv dependencies
RUN \
	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata

RUN \
	apt-get install -y \
	libgstreamer1.0-0 \
	gstreamer1.0-plugins-base \
	gstreamer1.0-plugins-good \
	gstreamer1.0-plugins-bad \
	gstreamer1.0-plugins-ugly \
	gstreamer1.0-libav \
	gstreamer1.0-doc \
	gstreamer1.0-tools \
	libgstreamer1.0-dev \
	libgstreamer-plugins-base1.0-dev


RUN apt-get install -y git

# just for testing
RUN apt-get -y install nano net-tools netcat

RUN apt-get update && apt-get install -y firefox

RUN apt-get install -y build-essential libssl-dev

RUN apt-get -y install cmake

# setup python
RUN apt-get install -y python3-pip

# install mavlink dependencies: https://github.com/ArduPilot/pymavlink
RUN apt-get install -y gcc python3-dev libxml2-dev libxslt-dev

RUN pip3 install  pymavlink torch==1.9.0 torchvision==0.10.0 opencv-python seaborn pandas ipython onnx==1.8.0 onnxruntime==1.8.0 pyaml tqdm 

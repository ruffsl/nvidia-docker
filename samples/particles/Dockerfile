FROM cuda:latest

WORKDIR /usr/local/cuda/samples/5_Simulations/particles
RUN make -j8

RUN apt-get update

RUN apt-get install -y \
	mesa-utils \
  libdbus-glib-1-2 \
  libgl1-mesa-dri \
  libgl1-mesa-glx

CMD ./particles

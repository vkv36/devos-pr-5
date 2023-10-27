FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
x11-apps 
# xauth \
# && rm -rf /var/lib/apt/lists/*
VOLUME [ "/run/desktop/mnt/host/wslg/.X11-unix:/tmp/.X11-unix" ]

ENV DISPLAY=:0
ENV WAYLAND_DISPLAY=wayland-0
ENV XDG_RUNTIME_DIR=/mnt/wslg/runtime-dir
ENV PULSE_SERVER=/mnt/wslg/PulseServer


CMD [ "xeyes" ]


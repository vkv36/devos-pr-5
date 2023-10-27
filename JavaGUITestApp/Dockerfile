FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
# x11-apps \
openjdk-11-jre

WORKDIR /home/
COPY calc.jar /home/

CMD [ "java","-jar", "calc.jar" ]

VOLUME [ "/run/desktop/mnt/host/wslg/.X11-unix:/tmp/.X11-unix" ]
VOLUME [ "/run/desktop/mnt/host/wslg:/mnt/wslg" ]

ENV DISPLAY=:0
ENV WAYLAND_DISPLAY=wayland-0
ENV PULSE_SERVER=/mnt/wslg/PulseServer



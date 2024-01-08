FROM ubuntu:22.04

RUN apt update && apt install -y ttyd openssh-server curl vim 

USER 10014
EXPOSE 7681 8080

CMD [ "ttyd", "-p", "8080", "-s", "3", "-t", "titleFixed=/bin/sh", "-t", "rendererType=webgl", "-t", "disableLeaveAlert=true", "/bin/sh", "-i", "-l" ]

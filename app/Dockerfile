FROM python:3.8.12-slim
#FROM python:3.7.3
WORKDIR /app
RUN apt-get update -y
# Installing the sources for the locales
#RUN  apt-get install glibc-locale-source -y
# Setting up the default locale to en_US.UTF-8
#RUN  localedef --no-archive -i en_US -f UTF-8 en_US.UTF-8 && \
      #export LANG=en_US.UTF-8
# Installing Necessary packages including firefox
#RUN  apt-get install dbus-x11 PackageKit-gtk3-module libcanberra-gtk2 -y
# Generating a universally unique ID for the Container
#RUN  dbus-uuidgen > /etc/machine-id
RUN apt-get install tk -y
RUN apt-get install python3 python3-pip -y
RUN pip3 install --upgrade Pillow
#RUN apt-get install -y Pillow
#RUN apt-get install python3-tkinter -y
# Starting Firefox application
CMD ["/app/tkinter_app.py"]
ENTRYPOINT ["python3"]

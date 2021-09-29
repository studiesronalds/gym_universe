FROM python:3.6-buster

ADD requirements.txt /opt/requirements.txt

WORKDIR /opt

RUN pip install -r ./requirements.txt

RUN apt-get update; apt-get install -y tmux htop cmake golang libjpeg-dev

RUN pip install "gym[all]"; \
	pip install universe; \
	pip install pyglet==1.3.2;
    
RUN pip install pyvirtualdisplay; \
	apt-get install -y xvfb; \
	pip install gym[Box_2D]; \
	pip install Box2D; \
    pip install gym-notebook-wrapper; \
    apt install -y freeglut3-dev;


FROM localhost:5000/universe

RUN apt-get install -y python3-dev; \
	pip install jupyter; \
	jupyter-lab; \
	pip install notebook;

CMD [ "xvfb-run", "--auto-servernum", "--server-num=1", "-s", "\"-screen 0 1400x900x24\"", "jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root" ]

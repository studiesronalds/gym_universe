FROM localhost:5000/universe

RUN apt-get install -y python3-dev; \
	pip install jupyter; \
	jupyter-lab; \
	pip install notebook;


CMD ["jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]
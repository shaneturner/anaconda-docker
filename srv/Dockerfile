FROM continuumio/anaconda3

ADD ./srv/conf/requirements.txt /

# RUN apt-get -y install gcc 
RUN pip install --upgrade setuptools && pip install -r requirements.txt
RUN mkdir -p /root/.jupyter
COPY ./srv/conf/jupyter_notebook_config.json /root/.jupyter/jupyter_notebook_config.json

EXPOSE 8888

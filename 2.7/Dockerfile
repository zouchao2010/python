FROM python:2.7

RUN apt-get update \
    && apt-get install -y wget unzip \
    && apt-get autoremove -y \
    && apt-get clean -y \
    && apt-get autoclean -y \
    && rm -rf /var/lib/apt/lists/*

RUN pip install tornado \
    && pip install thriftpy \
    && pip install toro \
    && pip install twilio \
    && pip install docopt \
    && pip install protobuf \
    && pip install sockjs-tornado \
    && pip install redis \
    && pip install tornado-redis \
    && pip install motor \
    && pip install PyJWT \
    && pip install eventlet \
    && pip install bcrypt \
    && pip install requests \
    && pip install momoko==1.1.5 \
    && pip install Pillow \

    && rm -rf /tmp/pip-*

# install pycoin
RUN wget https://github.com/richardkiss/pycoin/archive/master.zip \
    && unzip master.zip \
    && cd pycoin-master \
    && python setup.py install \
    && cd .. \
    && rm -rf master.zip pycoin-master

CMD ["python"]
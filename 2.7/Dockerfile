FROM python:2.7

RUN apt-get update \
    && apt-get install -y wget unzip libjpeg-dev \
    && apt-get autoremove -y \
    && apt-get clean -y \
    && apt-get autoclean -y \
    && rm -rf /var/lib/apt/lists/*

RUN pip install tornado --upgrade \
    && pip install thriftpy --upgrade \
    && pip install toro --upgrade \
    && pip install twilio --upgrade \
    && pip install docopt --upgrade \
    && pip install protobuf --upgrade \
    && pip install sockjs-tornado --upgrade \
    && pip install redis --upgrade \
    && pip install tornado-redis --upgrade \
    && pip install motor --upgrade \
    && pip install PyJWT --upgrade \
    && pip install eventlet --upgrade \
    && pip install bcrypt --upgrade \
    && pip install requests --upgrade \
    && pip install momoko --upgrade \
    && pip install Pillow --upgrade \
    && pip install python-dateutil --upgrade \
    && pip install asyncmc --upgrade \

    && rm -rf /tmp/pip-*

# install pycoin
RUN wget https://github.com/richardkiss/pycoin/archive/master.zip \
    && unzip master.zip \
    && cd pycoin-master \
    && python setup.py install \
    && cd .. \
    && rm -rf master.zip pycoin-master

CMD ["python"]

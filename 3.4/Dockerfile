FROM python:3.4

RUN apt-get update \
    && apt-get install -y wget vim tmux unzip gcc libjpeg-dev libffi-dev libpq-dev\
    && apt-get autoremove -y \
    && apt-get clean -y \
    && apt-get autoclean -y \
    && rm -rf /var/lib/apt/lists/*

RUN pip3.4 install pip --upgrade \
    && pip3.4 install setuptools --upgrade \
    && pip3.4 install tornado --upgrade \
    && pip3.4 install thriftpy --upgrade \
    && pip3.4 install toro --upgrade \
    && pip3.4 install twilio --upgrade \
    && pip3.4 install docopt --upgrade \
    && pip3.4 install protobuf --upgrade \
    && pip3.4 install sockjs-tornado --upgrade \
    && pip3.4 install redis --upgrade \
    && pip3.4 install tornado-redis --upgrade \
    && pip3.4 install motor --upgrade \
    && pip3.4 install PyJWT --upgrade \
    && pip3.4 install eventlet --upgrade \
    && pip3.4 install bcrypt --upgrade \
    && pip3.4 install requests --upgrade \
    && pip3.4 install momoko --upgrade \
    && pip3.4 install Pillow --upgrade \
    && pip3.4 install python-dateutil --upgrade \
    && pip3.4 install asyncmc --upgrade \
    && pip3.4 install psutil --upgrade \
    && pip3.4 install phonenumbers --upgrade \
    && pip3.4 install pyconvert --upgrade \
    && pip3.4 install Tornado-MySQL --upgrade \
    && pip3.4 install hyper --upgrade \
    && pip3.4 install bleach --upgrade \
    && pip3.4 install totoro --upgrade \
    && pip3.4 install gevent --upgrade \
    && pip3.4 install pycoin --upgrade \
    && pip3.4 install sqlalchemy --upgrade \
    && pip3.4 install ws4py --upgrade \
    && pip3.4 install config --upgrade \
    && pip3.4 install sqlautocode --upgrade \
    && pip3.4 install apscheduler --upgrade \
    && pip3.4 install threadspool --upgrade \

    && rm -rf /tmp/pip3.4-*

CMD ["python"]

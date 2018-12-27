#Image

FROM python:3.5-alpine

#ENV

ENV PYTHONUNBUFFERED=1
ENV WEBAPP_DIR=/src

#Custome Command
RUN mkdir -p /var/log/gunicorn
RUN mkdir $WEBAPP_DIR
WORKDIR $WEBAPP_DIR
ADD requirments.txt $WEBAPP_DIR/
RUN  pip install -r requirments.txt
ADD . $WEBAPP_DIR
RUN  python manage.py collectstatic
RUN  python manage.py migrate

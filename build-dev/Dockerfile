FROM python:3.6
LABEL maintainer 'Bruno Riwerson Silva <riwerson@gmail.com>'

RUN useradd www && \
  mkdir /app && \
  mkdir /log && \
  chown www /log

USER www
VOLUME /log
WORKDIR /app
EXPOSE 8000

ENTRYPOINT ["/usr/local/bin/python"]
CMD ["run.py"]

#Create: docker image build -t ex-build-dev .
#Start: docker container run -it -v $(pwd):/app -p 80:8000 --name python-server ex-build-dev

FROM  nginx:latest
LABEL maintainer 'Bruno Riwerson Silva <riwerson@gmail.com>'

RUN echo '<h1>Sem conteudo</h1>' > /usr/share/nginx/html/conteudo.html
COPY *.html /usr/share/nginx/html/

#Create: docker image build -t ex-build-copy .
#Start: docker container run -p 80:80 ex-build-copy

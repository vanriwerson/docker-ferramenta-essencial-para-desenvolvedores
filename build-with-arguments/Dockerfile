FROM debian
LABEL maintainer 'Bruno Riwerson Silva <riwerson@gmail.com>'

ARG S3_BUCKET=files
ENV S3_BUCKET=${S3_BUCKET}

#Create passing arg (key=value): docker image build --build-arg S3_BUCKET=myapp -t ex-build-arg .
#Execute: docker container run ex-build-arg bash -c 'echo $S3_BUCKET'
#Filter data on inspect: docker image inspect --format="{{index .Config.Labels \"maintainer\"}}" ex-build-arg
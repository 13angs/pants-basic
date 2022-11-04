# docker from docker refs: https://tomgregory.com/running-docker-in-docker-on-windows/
FROM python

WORKDIR /usr/src/app

# install the required packages
COPY ./ ./

RUN ./pants package src/python/api:app

# run docker as non-root user
# RUN adduser -D 13angs

# # run as 13angs
# USER 13angs
ENV TZ=Asia/Bangkok

CMD ./dist/src.python.api/app.pex
FROM cptactionhank/netatalk:latest

RUN groupadd -g1000 share
RUN useradd --no-create-home -u1000 -g1000 -G users share
RUN echo "share:share" | chpasswd

COPY ./afp.conf /etc/netatalk/afp.conf

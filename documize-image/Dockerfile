from alpine:3.11.3

RUN mkdir /opt/documize
COPY ./documize.conf /opt/documize/.

WORKDIR /opt/documize

RUN wget https://github.com/documize/community/releases/download/v3.7.0/documize-community-linux-amd64

RUN chmod o+x documize-community-linux-amd64

# since we name conf file as documize.conf we dont need to pass it along
CMD ["./documize-community-linux-amd64"]
EXPOSE 8080

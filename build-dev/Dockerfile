FROM python:3.6
LABEL maintainer 'Aluno Cod3r <aluno at cod3r.com.br>'

RUN useradd WWW && \
    mkdir /app && \
    mkdir /log && \
    chown WWW /log

USER WWW
VOLUME /log
WORKDIR /app
EXPOSE 8000

ENTRYPOINT [ "/usr/local/bin/python" ]
CMD [ "run.py" ]
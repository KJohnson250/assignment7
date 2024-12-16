FROM ubuntu:latest

RUN mkdir -p /structure && chmod 777 /structure
RUN useradd -u 5000 collin
RUN useradd sync
RUN useradd nobody

RUN touch /structure/sync-work && chown sync:sync /structure/sync-work
RUN touch /structure/nobody-work && chown nobody:nogroup /structure/nobody-work

CMD ["sh", "-c", "while true; do echo users; done"]

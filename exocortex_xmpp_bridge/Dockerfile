FROM python:3.12-alpine
LABEL application="Exocortex XMPP Bridge"

COPY requirements.txt /app/
RUN set -x && \
    apk update && \
    apk add --no-cache --virtual .build-deps gcc musl-dev libffi-dev && \
    pip install --no-cache-dir -r /app/requirements.txt && \
    apk del .build-deps

ADD . /app/
EXPOSE 8003
WORKDIR /app
USER nobody
CMD ["python3", "exocortex_xmpp_bridge.py"]

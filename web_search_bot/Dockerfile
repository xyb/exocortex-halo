FROM python:3.12-alpine
LABEL application="Exocortex XMPP Bridge"

COPY requirements.txt /app/
RUN set -x && \
    pip install --no-cache-dir -r /app/requirements.txt

ADD . /app/
WORKDIR /app
USER nobody
CMD ["python3", "web_search_bot.py"]

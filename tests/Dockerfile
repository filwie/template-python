FROM python:3.7-alpine

WORKDIR /opt/test
COPY . .
RUN apk add git && \
    pip install -r requirements.txt && \
        pip install -r test_requirements.txt && \
        python setup.py install

ENTRYPOINT ["pytest"]
CMD ["-v"]

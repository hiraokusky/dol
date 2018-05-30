FROM alpine:3.5

LABEL @hiraokusoy <>

RUN apk add --no-cache --virtual --update py-pip make wget ca-certificates ttf-dejavu \
    && pip install --upgrade pip \
    && pip install sphinx commonmark==0.5.4 recommonmark sphinx-autobuild sphinx_rtd_theme sphinxcontrib-mermaid

WORKDIR /work

EXPOSE 8000 18000

CMD echo "hello, sphinx!"
FROM httpd:alpine
RUN apk add --no-cache apcupsd-webif
COPY ./httpd.conf /usr/local/apache2/conf/httpd.conf
COPY ./apcupsd.css /etc/apcupsd/apcupsd.css
COPY ./multimon.conf /etc/apcupsd/multimon.conf
COPY ./entrypoint.sh /usr/local/bin/
CMD ["/usr/local/bin/entrypoint.sh"]

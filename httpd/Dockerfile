FROM base/arch
RUN pacman --noconfirm -Sy apache supervisor
ADD httpd.ini /etc/supervisor.d/httpd.ini
ADD index.html /srv/http/index.html
EXPOSE 80
CMD ["/usr/bin/supervisord"]

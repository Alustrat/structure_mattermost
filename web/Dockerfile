FROM nginx:mainline

RUN rm /etc/nginx/conf.d/default.conf
ADD https://raw.githubusercontent.com/Alustrat/structure_mattermost/master/web/mattermost /etc/nginx/sites-available/
ADD https://raw.githubusercontent.com/Alustrat/structure_mattermost/master/web/mattermost-ssl /etc/nginx/sites-available/

ADD https://raw.githubusercontent.com/Alustrat/structure_mattermost/master/web/docker-entry.sh /
RUN chmod +x /docker-entry.sh
ENTRYPOINT /docker-entry.sh

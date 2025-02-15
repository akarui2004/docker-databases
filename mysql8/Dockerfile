ARG VERSION=8
FROM mysql:${VERSION}

# Set timezone
ARG TZ=UTC
ENV TZ ${TZ}
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone && chown -R mysql:root /var/lib/mysql/

## MySQL 5.7 shouldn't copy the my.cnf because this file is for mysql 8.0
# MySQL config file
COPY my.cnf /etc/mysql/conf.d/my.cnf

# Set the permission for the config file
RUN chmod 0444 /etc/mysql/conf.d/my.cnf

CMD ["mysqld"]

EXPOSE 3306

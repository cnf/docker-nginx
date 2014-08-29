# Nginx Dockerfile

Just the basics

## Running it

    docker run -d --name nginx-conf --volume /etc/nginx/sites-enabled --volume /etc/nginx/conf.d busybox:latest /bin/true
    docker run -t -i --rm --volumes-from nginx-conf --net=host frosquin/nginx

# About this Repo

This is the Git repo of the unofficial Docker image for nginx-reverse-proxy.

## Usage
1. Clone the git repo.

2. Customize your `server_name` and `proxy_pass` at `/etc/nginx/conf.d/default.conf` file.

3. Customize your nginx settings at `/etc/nginx/conf.d/default.conf` and `/etc/nginx/nginx.conf` files.

4. Build a Docker image
```sh
$ docker build -t {image name} .
```

5. Start your Docker container
```sh
$ docker run -d -p 80:80 {image name}
```

# Using GitLab with SSL enabled integrated with NGINX proxy and autorenew LetsEncrypt certificates

This docker-compose should be used with WebProxy (the NGINX Proxy):

[https://github.com/evertramos/docker-compose-letsencrypt-nginx-proxy-companion](https://github.com/evertramos/docker-compose-letsencrypt-nginx-proxy-companion)


## Usage

After everything is settle, and you have your three containers running (_proxy, generator and letsencrypt_) you do the following:

1. Clone this repository.

2. Make a copy of our .env.sample and rename it to .env:

Update this file with your preferences.

>This container must use a network connected to your webproxy or the same network of your webproxy.

3. Start your project

```bash
docker-compose up -d
```

**Be patinet** - when you first run a container to get new certificates, it may take a few minutes.

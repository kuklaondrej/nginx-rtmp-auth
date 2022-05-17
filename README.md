# nginx-rtmp-auth
A Python script that allows you to authenticate RTMP publishers in nginx-rtmp-module.

## Usage:
- Build NGINX with nginx-rtmp-module and see [the example conf](/example-nginx.conf) for how to setup authentication with the script.
- Install dependencies: `pip3 install -r requirements.txt`
- Edit [config.ini](/config.ini) with general settings, then edit [authentication.json](/authentication.json) with your applications and stream names (also called stream keys)
- Run with `sudo python3 rtmpauth.py` (sudo not needed if you are using a port number over 1000)

## config.ini:

```
[main]
bind_to_ip = 127.0.0.1 # IP address to bind to
bind_to_port = 88 # Port to bind to
authentication_file = authentication.json
log_to_file = auth.log # File to log to - basically an access.log
```

## Getting Help:
If you need help, just open a new issue and describe with as much detail as possible the issue you are having. We will get back to you as soon as possible.

## IRLTookit Links

- https://twitter.com/IRLToolkit
- https://irltoolkit.com/discord
- https://irltoolkit.com

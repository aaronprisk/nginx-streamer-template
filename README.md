# NGINX Streamer BastilleBSD Template
BastilleBSD Template for quickly spinning up NGINX-RTMP-VideoJS containers for live video streaming purposes.

## Installing Template
Using the template is super easy. Simply run the following commands on a FreeBSD system with Bastille installed:
```
bastille bootstrap https://github.com/aaronprisk/nginx-streamer-template
```
You can now apply the template to a running Bastille container via:
```
bastille template TARGET aaronprisk/nginx-streamer-template
```
## Configuration
The template comes with all the essential building blocks required for a simple live video streaming server, however some additional configuration is required before you can go live. 

* In the provided player template (/usr/local/www/index.html) you'll need to insert your servers IP address in the video source line.
* You may want to adjust the RTMP settings in the provided nginx config (/usr/local/etc/nginx/nginx.conf) to fit your streaming needs. 

## Resources
You can find more information on live streaming with this stack here: https://opensource.com/article/20/2/video-streaming-tools

FROM nextcloud:fpm-alpine
RUN apk update && apk add ffmpeg imagemagick ghostscript unrar p7zip
RUN sed -i 's/\(^ *<policy.*rights="\)\([^"]*\)\(".*PDF.*\/>\)/\1read|write\3/1' /etc/ImageMagick-7/policy.xml
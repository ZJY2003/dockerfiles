FROM bitnami/minideb
MAINTAINER TONY ZOU<tony200303.zt@gmail.com>

ENV MOD_NODEID = 1   \
    MOD_KEY = mupass  \
    V2RAY_ALTERID = 10  \
    V2RAY_TAG = proxy

ADD bin /root/v2ray/
ADD https://files.indexyz.me/Resource/V2Ray/v2ray /root/v2ray/
ADD https://files.indexyz.me/Resource/V2Ray/v2ctl /root/v2ray/

RUN cd /root/v2ray && \
    chmod +x bin v2ray v2ctl
WORKDIR /root/v2ray
CMD /root/v2ray/bin

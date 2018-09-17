FROM ambakshi/perforce-base
MAINTAINER Amit Bakshi <ambakshi@gmail.com>

ENV P4P_VERSION 15.2
ENV REFRESHED_AT 2016-05-14

RUN curl -sSL -O https://notsa-my.sharepoint.com/:u:/g/personal/nigel_clark_coltellait_com/EXBg9m1rwL1PlrCkRb-qzBcB-U0axPuGIqQMSEgH_QlqXw?e=LWKxUh && mv p4 /usr/bin/p4 && chmod +x /usr/bin/p4
RUN curl -sSL -O https://notsa-my.sharepoint.com/:u:/g/personal/nigel_clark_coltellait_com/EVgWCrDYje9Fr0_InVXrCAIButPHATZVFzVFGNwjKUpPbw?e=4dB8H6 && mv p4p /usr/bin/p4p && chmod +x /usr/bin/p4p

ENV P4TARGET perforce:1666
ENV P4PORT 1666
ENV P4PCACHE /cache

VOLUME ["$P4PCACHE"]

EXPOSE 1666

CMD ["/usr/bin/p4p"]

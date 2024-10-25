FROM alpine

# Maintained by: Alex Sylvis

# Add repo file
ADD ./alpmap.repo /etc/apk/repositories

# Install packages
RUN apk add bash nmap

ENTRYPOINT [ "/usr/bin/nmap" ]
CMD [ "-sn","172.17.0.0/24" ]

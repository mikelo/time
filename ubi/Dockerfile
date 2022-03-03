FROM registry.access.redhat.com/ubi8/ubi
MAINTAINER Veer Muchandi veer@redhat.com
ADD ./init.sh ./
RUN dnf install nmap-ncat -y 
RUN chown 1001:1001 init.sh && chmod o+w init.sh
USER 1001
EXPOSE 8080
CMD ["./init.sh"]

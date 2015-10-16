FROM centos:centos7
MAINTAINER Jura Berg <jura.berg@nebula.fi>
RUN yum install -y https://repos.fedorapeople.org/repos/openstack/openstack-juno/rdo-release-juno-1.noarch.rpm && yum install -y epel-release
RUN yum install -y python-novaclient \
    python-neutronclient \
    python-heatclient \
    git

ENV AUTH_URL "https://identity.fi-1.nebulacloud.fi:5000/v2.0"
ENV REGION "fi-1"

COPY openrc-test /openrc-test

CMD ["bash"]

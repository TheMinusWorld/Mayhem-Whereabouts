#
# This Dockerfile sets up the container for Mayhem Whereabouts deployment
#
# Dockerfile documentation is available here: https://docs.docker.com/engine/reference/builder/
#
FROM centos:8.1.1911

# Install Extra Packages for Enterprise Linux repo & update packages
# EPEL documentation is available at https://fedoraproject.org/wiki/EPEL
RUN dnf -y install epel-release && \
  dnf -y update

# Install Ansible - an environment management tool
# See documentation at https://docs.ansible.com/ansible/latest/index.html
RUN dnf -y install ansible

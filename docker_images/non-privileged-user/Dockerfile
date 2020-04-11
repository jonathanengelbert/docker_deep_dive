# Creates a CentOS image that uses cloud_user as non-privileged user

FROM centos:latest
RUN useradd -ms /bin/bash cloud_user
# RUN, CMD and ENTRYPOINTS THAT FOLLOW THE NEXT STATEMENT WILL BE EXECUTED AS
# THE USER SPECIFIED BELOW
USER cloud_user

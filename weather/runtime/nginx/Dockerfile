FROM registry.redhat.io/rhel8/nginx-116

# the maintainer
LABEL maintainer="Marcus Maestri <mmaestri@redhat.com>" \
    # specify where s2i scripts are located
    io.openshift.s2i.scripts-url="image:///usr/libexec/s2i/bin"

# s2i scripts
COPY s2i /usr/libexec/s2i

# default user
USER 1001

# Set the default command for the resulting image
CMD /usr/libexec/s2i/run
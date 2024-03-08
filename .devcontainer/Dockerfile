# Use Red Hat Universal Base Image (UBI) as a base
FROM registry.access.redhat.com/ubi8/ubi

# Set metadata
LABEL maintainer="Pythonemus"

# Install Python 3 and development tools
RUN yum -y install python3 python3-devel python3-pip gcc openssl-devel libffi-devel

# Install Ansible using pip
RUN pip3 install --upgrade pip
RUN pip3 install ansible

# Set the working directory inside the container
WORKDIR /workspace

# Copy any additional files or scripts if needed
# COPY . .

# Set default command to launch bash
CMD ["bash"]

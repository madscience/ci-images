FROM circleci/node:12.16-buster

# Install sentry-cli
RUN sudo npm install -g @sentry/cli --unsafe-perm

# Install Python PIP
RUN sudo apt-get update && sudo apt-get install -y python3-pip

# Install cfn-lint
RUN pip3 install cfn-lint

# Install tf-helper
RUN curl -SL https://github.com/hashicorp-community/tf-helper/archive/0.2.8.tar.gz | tar -xzC ~/ \
    && sudo ln -s ~/tf-helper-0.2.8/tfh/bin/tfh /usr/local/bin/tfh

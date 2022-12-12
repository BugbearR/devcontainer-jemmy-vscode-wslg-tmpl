FROM mcr.microsoft.com/devcontainers/base:jammy

USER root
RUN apt-get update -y \
    && DEBIAN_FRONTEND=noninteractive apt-get upgrade -y \
    && apt-get clean \
    && rm -rf /var/cache/apt/* /var/lib/apt/lists/

USER vscode
RUN mkdir -m 700 ~/.xdg

CMD [ "/bin/bash" ]

ARG JAVA_VERSION=17

FROM eclipse-temurin:${JAVA_VERSION}

WORKDIR /usr/src/app

RUN sh -c "$(wget -O- https://github.com/deluan/zsh-in-docker/releases/download/v1.1.5/zsh-in-docker.sh)" -- \
    -t robbyrussell \
    -p https://github.com/zsh-users/zsh-autosuggestions \
    -p https://github.com/zsh-users/zsh-syntax-highlighting \
    -p https://github.com/zsh-users/zsh-completions \
    -p https://github.com/rupa/z/

EXPOSE 8080

CMD [ "zsh"]

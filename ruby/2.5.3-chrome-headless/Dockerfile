FROM ruby:2.5.3

# Install google chrome dependencies and install google chrome stable
RUN apt-get update && apt-get -y install libappindicator3-1 libasound2 \
        libatk-bridge2.0-0 libgtk-3-0 libx11-xcb1 libxss1 libxtst6 xdg-utils \
        fonts-liberation lsb-release libnss3 libnspr4 && \
    wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb && \
    dpkg -i google-chrome*.deb && \
    rm google-chrome*.deb && \
    apt-get -y autoremove
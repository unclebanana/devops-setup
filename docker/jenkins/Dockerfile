FROM jenkins:2.7.1


USER root

## Android SDK tools
# http://stackoverflow.com/questions/18928164/android-studio-cannot-find-aapt/18930424#18930424
RUN apt-get update && apt-get install -y lib32stdc++6 lib32z1 && apt-get clean && rm -rf /var/lib/apt/lists/*

USER jenkins

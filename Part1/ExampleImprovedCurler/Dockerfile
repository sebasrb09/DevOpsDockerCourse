FROM ubuntu:20.04

RUN apt-get -y update
RUN apt-get -y install curl

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy the script.sh file from this location to /usr/src/app/ creating /usr/src/app/script.sh
COPY script.sh .

# Alternatively, if we skipped chmod earlier, we can add execution permissions during the build.
RUN chmod +x script.sh

# Execute a command with `/bin/sh -c` prefix.
#RUN touch additional.txt
ENTRYPOINT [ "./script.sh" ]
# When running docker run the command will be ./script.sh
CMD ["helsinki.fi"]
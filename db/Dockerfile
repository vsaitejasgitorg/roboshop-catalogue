FROM            redhat/ubi9
COPY            mongo.repo /etc/yum.repos.d
RUN             dnf install mongodb-mongosh git -y
RUN             mkdir /app
WORKDIR         /app
COPY            *.js run.sh /app/
ENTRYPOINT      ["bash", "run.sh"]

FROM postman/newman
COPY *.json /etc/newman/*.json
CMD [ "run", "*.json", "-r", "cli,junit" ]
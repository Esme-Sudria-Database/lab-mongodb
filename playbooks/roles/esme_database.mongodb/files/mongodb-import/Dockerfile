# see https://github.com/dexteryy/nodecube-example/blob/master/configs/Dockerfile-mongoimport

FROM mongo:4.2.1-bionic

ADD cities15000.json \
  /tmp/

CMD until echo 'db.stats().ok' | mongo admin --host localhost --quiet; \
    do sleep 1; \
  done && \
  mongo geography \
  --host localhost \
  --eval "db.dropDatabase();" && \
  # NOTE: keep the above lines
  mongoimport \
  --host localhost \
  --db geography \
  --collection cities \
  --type json \
  --jsonArray \
  --file /tmp/cities15000.json; \

Set `HOST` in `bin/ou.env` to the ip of your host where you're running openunison

Build Test
`cd app;mvn clean package;cd ..`

Create Image
`s2i build app/target tremolosecurity/openunisons2idocker  local/openunison`

Run Image
`docker run -ti -p 8443:8443 -v /Users/mlb/git-local/undertow-memory-issue/bin:/etc/openunison:Z -e JAVA_OPTS='-XX:+UseParallelGC -Djava.awt.headless=true -Djava.security.egd=file:/dev/./urandom -Xmx1G -Xms1G' --name openunison local/openunison`
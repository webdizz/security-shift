# security-shift
Demo related artifacts to support "Security. Level Up" talk


## Download sample site jar
`wget -c https://github.com/continuumsecurity/RopeyTasks/raw/master/ropeytasks.jar`

## Start application
`java -jar ropeytasks.jar`

## Run Docker container
`docker run --name=tiger -v `pwd`/report.html:/tmp/report.html:rw --network host -d -e host=host.docker.internal -e port=8080 -e protocol=http --rm TODO`

## Execute scanning 
`docker exec -t tiger run -s basic`

## Stop container
`docker kill tiger`

## Open report
`open report.html`

# security-shift
Demo related artifacts to support "Security. Level Up" talk


## Download sample site jar
`wget -c https://github.com/continuumsecurity/RopeyTasks/raw/master/ropeytasks.jar`

## Start application
`java -jar ropeytasks.jar`

## Run Docker container along with running 'basic' test
`docker run -v `pwd`:/tmp/reports:rw --network host -e project_name=ropeytasks -e environment=local -e host=host.docker.internal -e port=8080 -e protocol=http --rm TODO -s basic`

## Open report, there will be a file generated based on name of project and environment. In our case 'TEST-ropeytasks-local-basic.html'.
`open TEST-ropeytasks-local-basic.html`

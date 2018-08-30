# Docker

## Docker best practices
1. Use official repos when possible
2. Keep your images small
3. Be specific with your image versions (don't use latest in production)


## Dockerfile notes
* Instructions for building images
* CAPITALIZE instructions
* <INSTRUCTION> <value>
* FROM always first instruction
* FROM = base image
* Good practice to list maintainer
* RUN = execute command and create layer
* COPY = copy code into image as new layer
* Some instructions add metadata instead of layers
* ENTRYPOINT = default app for image/container

## Logging
* Applications should send their logs to STDOUT and STDERR.  
	* From those locations, we can add plugins that will allow, for instance Splunk, to read those logs

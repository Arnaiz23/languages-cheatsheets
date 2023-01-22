# Docker cheatsheet

## Docker run

```bash
	--name "name" -> select the name of the container
	-d -> detach mode
	-it image bash -> run and open bash
	-p host:container -> open ports
	-v /volumeHost:/volumeContainer -> create volumes
```

## Docker Copy

`docker cp route container:route`
`docker cp container:route route`


## Examples

```bash
# Mongo
	docker run -d --name tu-compra-mongo -p 27017:27017 mongo
```
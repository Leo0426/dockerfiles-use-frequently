# Dockerfile frequently used in daily work

## Use docker build command to build dockerfile

### usage: 

```
    docker build [options] path | url | -
```

### some useful options : 
|     option name      | description  |
|  :--------------:  | :--------------:  |
| -- file , -f		| Name of the Dockerfile (Default is ‘PATH/Dockerfile’)
| -- no-cache		| Do not use cache when building the image
| -- output , -o	| API 1.40+ , Output destination (format: type=local,dest=path)
| -- platform		| API 1.38+ , Set platform if server is multi-platform capable
| -- pull		    | Always attempt to pull a newer version of the image
| -- quiet , -q		| Suppress the build output and print image ID on success
| -- rm	true	    | Remove intermediate containers after a successful build
| -- tag , -t		| Name and optionally a tag in the ‘name:tag’ format
| -- target		    | Set the target build stage to build.

### Examples
```
docker built -t company/jdk:8 -f alpine_jdk/Dockerfile .
```

### Note
- Each one has been tested and can be used normally
- Some dockerfile only for study, recommend to use official images
- please contact me if you have any questions
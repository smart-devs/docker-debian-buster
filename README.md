# Debian Buster base image

This Repo contains the build instructions for the Debian Stretch base image. All images should inherit from this image.

## Documentation

This image is automatically build with following cron expression `0 0 * * *`.

### Environment vars

| Argument                              | Default Value                                             | Description |
| :---                                  | :---                                                      | :---         |

### Build Arguments

All build arguments can be prefixed with `DOCKER_BUILD_ARG_`. For testing you can also set them directly during docker build as `--build-arg=` argument. 

note: `DOCKER_BUILD_ARG_` prefix can be prepend to all shown variables to replace their defaults.

| Argument                              | Default Value                                                 | Description |
| :---                                  | :---                                                          | :---         |
| FROM                                  | debian:buster-slim                                           | Base image to build from |
| CONTAINER_RUNTIME_REQUIREMENTS        | less procps ca-certificates                                   | Packages for container during runtime |
| CONTAINER_BUILD_REQUIREMENTS          | curl                                                          | Packages for container required during build |
| CONTAINER_RUNTIME_REQUIREMENTS_EXTRA  | *empty                                                        | extra runtime requirements |
| CONTAINER_BUILD_REQUIREMENTS_EXTRA    | *empty                                                        | extra build requirements |

## Contributing

## Changelog
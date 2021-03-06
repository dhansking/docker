% DOCKER(1) Docker User Manuals
% Docker Community
% JUNE 2014
# NAME
docker-exec - Run a command in a running container

# SYNOPSIS
**docker exec**
[**-d**|**--detach**[=*false*]]
[**-i**|**--interactive**[=*false*]]
[**-t**|**--tty**[=*false*]]
CONTAINER COMMAND [ARG...]

# DESCRIPTION

Run a process in a running container. 

The command started using `docker exec` will only run while the container's primary
process (`PID 1`) is running, and will not be restarted if the container is restarted.

If the container is paused, then the `docker exec` command will wait until the
container is unpaused, and then run

# OPTIONS
**-d**, **--detach**=*true*|*false*
   Detached mode: run command in the background. The default is *false*.

**-i**, **--interactive**=*true*|*false*
   Keep STDIN open even if not attached. The default is *false*.

**-t**, **--tty**=*true*|*false*
   Allocate a pseudo-TTY. The default is *false*.

# HISTORY
November 2014, updated by Sven Dowideit <SvenDowideit@home.org.au>

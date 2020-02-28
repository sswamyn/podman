% podman-volume-inspect(1)

## NAME
podman\-volume\-inspect - Get detailed information on one or more volumes

## SYNOPSIS
**podman volume inspect** [*options*] *volume* [...]

## DESCRIPTION

Display detailed information on one or more volumes. The output can be formatted using
the **--format** flag and a Go template. To get detailed information about all the
existing volumes, use the **--all** flag.
Volumes can be queried individually by providing their full name or a unique partial name.


## OPTIONS

**-a**, **--all**

Inspect all volumes.

**--format**=*format*

Format volume output using Go template

**--help**

Print usage statement


## EXAMPLES

```
$ podman volume inspect myvol

$ podman volume inspect --all

$ podman volume inspect --format "{{.Driver}} {{.Scope}}" myvol
```

## SEE ALSO
podman-volume(1)

## HISTORY
November 2018, Originally compiled by Urvashi Mohnani <umohnani@redhat.com>
#### Word Order

`SUBJECT TIME PLACE PREPOSITION VERB OBJECT`

e.g.:

> Gimli yesterday at Helm's Deep with Legolas smote some orcs.

Here's the `man` page:

```shell
KILL(1)                         User Commands                        KILL(1)
NAME         top

       kill - terminate a process
SYNOPSIS         top

       kill [-signal|-s signal|-p] [-q value] [-a] [--] pid|name...
       kill -l [number] | -L
DESCRIPTION         top

       The command kill sends the specified signal to the specified
       processes or process groups.  If no signal is specified, the TERM
       signal is sent.  This TERM signal will kill processes that do not
       catch it; for other processes it may be necessary to use the KILL
       signal (number 9), since this signal cannot be caught.

       Most modern shells have a builtin kill function, with a usage rather
       similar to that of the command described here.  The --all, --pid, and
       --queue options, and the possibility to specify processes by command
       name, are local extensions.

       If signal is 0, then no actual signal is sent, but error checking is
       still performed.
ARGUMENTS         top

       The list of processes to be signaled can be a mixture of names and
       pids.

       pid    Each pid can be one of four things:

              n      where n is larger than 0.  The process with pid n is
                     signaled.

              0      All processes in the current process group are
                     signaled.

              -1     All processes with a pid larger than 1 are signaled.

              -n     where n is larger than 1.  All processes in process
                     group n are signaled.  When an argument of the form
                     '-n' is given, and it is meant to denote a process
                     group, either a signal must be specified first, or the
                     argument must be preceded by a '--' option, otherwise
                     it will be taken as the signal to send.

       name   All processes invoked using this name will be signaled.
```

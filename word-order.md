#### Word Order

`SUBJECT TIME PLACE PREPOSITION VERB OBJECT`

e.g.:

> Gimli yesterday at Helm's Deep with Legolas smote some orcs.

Here's the `man` page:

```shell
MANDARIN(1)                User Commands                     MANDARIN(1)
NAME

       manarin - communications protocol
SYNOPSIS

       mandarin: [subject] [verb] [object]
       mandarin: subject [time] [place] [preposition] verb object
       
DESCRIPTION

       the mandarin protocol allows the users to communicate using short
       phrases of meaning.

       Most modern Chinese people can communicate using this protocol.
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

#### Word Order


> Gimli yesterday at Helm's Deep with Legolas smote some orcs.

Here's the `man` page:

```shell
MANDARIN(1)                User Commands                     MANDARIN(1)
NAME

       manarin - natural-language protocol
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

NOTES         top

       It is not possible to send a signal to an explicitly selected thread
       in a multithreaded process using the kill(2) syscall.  If kill(2) is
       used to send a signal to a thread group, then the kernel selects an
       arbitrary member of the thread group that has not blocked the signal.
       For more details see clone(2), the CLONE_THREAD description.

       The command kill(1) as well as syscall kill(2) accept a TID (thread
       ID, see gettid(2)) as an argument.  In this case the kill behavior is
       not changed and the signal is also delivered to the thread group
       rather than to the specified thread.

RETURN CODES

       kill has the following return codes:

       0      success

       1      failure

       64     partial success (when more than one process specified)
SEE ALSO

       Cantonese, Sichuanese, Shanghainese

AUTHORS

       Public Domain

       The original version was developed during the Shang Dynasty

AVAILABILITY

       The protocol has 955 million users worldwide.
```

1. [Help](#help)
2. [History](#history)
3. [Several commands](#several-commands)
4. if-else
5. loop
6. read file

## Help
```bash

man bash

man builtin

# help on builtin command 'history'
help history
```

## History
```bash

# show last N commands from bash history
history N
```

```bash
!!   repeat the previous line

# arguments
!*   all arguments
!:0  the command
!^   first argument
!$   last argument
!:N  N-th argument

!:2-4   2 to 4 arguments
!:2-$   2 to last arguments
!:2*    2 to last arguments
!:2-    2 to next to last arguments

```

## Several commands
* `A; B` - run A and then run B, regardless of A failed or succeeded
* `A && B` - run A and if A **succeeded** then run B
* `A || B` - run A and if A **failed** then run B
* `A &` - run A in background
* `(A ; B)` - concatenate output of A and B 
* `(cd A ; ls -lh)` - change directory to `A` and perform `ls` without changing directory


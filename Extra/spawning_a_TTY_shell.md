## TTY shell spawning
----------------------

> During pen tests or after an escalation, you may obtain a shell without tty (teletype). A tty is the Unix device name for physical or virtual terminal connection, the shell is the Unix command interpreter. To interact with the system, here are some commands which will allow you to spawn a tty shell. Some of those commands will depend on the system environment and installed packages.


### Shell Spawning

Python

```python
python -c 'import pty; pty.spawn("/bin/bash")'
python3 -c 'import pty; pty.spawn("/bin/bash")'
``` 

Bash

```bash   
echo os.system('/bin/bash')
/bin/sh -i
``` 
 
Perl

```perl
perl -e 'exec "/bin/sh";'
```

Lua

```lua
Lua 5.3.3  Copyright (C) 1994-2016 Lua.org, PUC-Rio
> os.execute('/bin/sh')
$
``` 

From within IRB (Interactive Ruby Shell)

```ruby
irb(main):001:0> exec "/bin/sh"
$
```

From within vi, vim

```vim
:!bash
:set shell=/bin/bash:shell
``` 

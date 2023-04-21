# Jaseci Cheatsheet - Work In Progess

- Jaseci Runtime CLI Commands - I am calling @jaseci > help (the command) in my Ubuntu terminal.

actions    booktool  global  jsorc   logout  prometheus  sentinel  wapi
alias      clear     graph   load    ls      publogin    service
apply      config    info    logger  master  reset       user
architype  edit      jac     login   object  script      walker

```yml
Command:
```
# actions

```bash
@jaseci > help actions
Usage: actions [OPTIONS] COMMAND [ARGS]...

  Group of `actions` commands

Options:
  --help  Show this message and exit.

Commands:
  call    Call an action by name
  list    List a set of or all loaded jaseci actions
  load    Group of `actions load` commands
  module  Group of `actions module` commands
  unload  Group of `actions unload` commands
```

```yml
Command:
```
# alias
  
```bash
@jaseci > help alias
Usage: alias [OPTIONS] COMMAND [ARGS]...

  Group of `alias` commands

Options:
  --help  Show this message and exit.

Commands:
  clear     Remove all string to string alias that client can use.
  delete    Delete an active string to string alias mapping.
  list      List all string to string alias that caller can use.
  register  Create string to string alias mapping that caller can use.
```

```yml
Command:
```
# apply

```bash
@jaseci > help apply
Usage: apply [OPTIONS] COMMAND [ARGS]...

  Group of `apply` commands

Options:
  --help  Show this message and exit.

Commands:
  yaml  apply manifest yaml to specific service
```

```yml
Command:
```
# architype

```bash
@jaseci > help architype
Usage: architype [OPTIONS] COMMAND [ARGS]...

  Group of `architype` commands

Options:
  --help  Show this message and exit.

Commands:
  count     Return count of architypes
  delete    Permanently delete sentinel with given id
  get       Get an architype rendered with specific mode
  list      List architypes known to sentinel
  register  Create an architype based on the code passed and return object.
  set       Set code/ir for a architype
```

```yml
Command:
```
# booktool

```bash
@jaseci > help booktool
Usage: booktool [OPTIONS] OP

  Internal book generation tools

Options:
  -o, --output TEXT  Filename to dump output of this command call.
  --help             Show this message and exit.
```

```yml
Command:
```
#

```bash

```

```yml
Command:
```
#

```bash

```

```yml
Command:
```
#

```bash

```

```yml
Command:
```
#

```bash

```





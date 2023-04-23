# Jaseci Cheatsheet

- Jaseci Runtime CLI Commands - I am calling @jaseci > help (the command) in my Ubuntu terminal.

| Commands| | | | | | | |
| --- | --- | --- | --- | --- | --- | --- | --- |
| actions | booktool | global | jsorc | logout | prometheus | sentinel | wapi |
| alias | clear | graph | load | ls | publogin | service |
| apply | config | info | logger | master | reset | user |
| architype | edit | jac | login | object | script | walker |

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
# clear

```bash
@jaseci > help clear
Usage: clear [OPTIONS]

  Clear terminal

Options:
  --help  Show this message and exit.
```

```yml
Command:
```
# config

```bash
@jaseci > config
Usage: config [OPTIONS] COMMAND [ARGS]...

  Group of `config` commands

Options:
  --help  Show this message and exit.

Commands:
  delete  Delete a config
  exists  Check a config is present
  get     Get a config
  index   List all valid configs
  list    Check a config is present
  set     Set a config
  update  Update a key-value of a config
```

```yml
Command:
```
# edit

```bash
@jaseci > help edit
Usage: edit [OPTIONS] FILE

  Edit a file

Options:
  --help  Show this message and exit.
```

```yml
Command:
```
# global

```bash
@jaseci > help global
Usage: global [OPTIONS] COMMAND [ARGS]...

  Group of `global` commands

Options:
  --help  Show this message and exit.

Commands:
  delete    Delete a global
  get       Get a global var
  sentinel  Group of `global sentinel` commands
  set       Set a global
```

```yml
Command:
```
# graph

```bash
@jaseci > help graph
Usage: graph [OPTIONS] COMMAND [ARGS]...

  Group of `graph` commands

Options:
  --help  Show this message and exit.

Commands:
  active  Group of `graph active` commands
  create  Create a graph instance and return root node graph object
  delete  Permanently delete graph with given id
  get     Return the content of the graph with mode Valid modes:...
  list    Provide complete list of all graph objects (list of root node...
  node    Group of `graph node` commands
  walk
```

```yml
Command:
```
# info

```bash
@jaseci > help info
Usage: info [OPTIONS]

  Provide information about this instance of Jaseci

Options:
  -o, --output TEXT  Filename to dump output of this command call.
  --help             Show this message and exit.
```

```yml
Command:
```
# jac 

```bash
@jaseci > help jac
Usage: jac [OPTIONS] COMMAND [ARGS]...

  Group of `jac` commands

Options:
  --help  Show this message and exit.

Commands:
  build  Command line tooling for building executable jac ir
  disas  Command line tooling for print IR for both .jac code files and...
  dot    Command line tooling for a walker then output graph in both .jac...
  run    Command line tooling for running all test in both .jac code...
  test   Command line tooling for running all test in both .jac code...
```

```yml
Command:
```
# jsorc

```bash
@jaseci > help jsorc
Usage: jsorc [OPTIONS] COMMAND [ARGS]...

  Group of `jsorc` commands

Options:
  --help  Show this message and exit.

Commands:
  actionpolicy  Group of `jsorc actionpolicy` commands
  actions       Group of `jsorc actions` commands
  benchmark     Group of `jsorc benchmark` commands
  loadtest      load test API.
  trackact      Group of `jsorc trackact` commands
  tracksys      Group of `jsorc tracksys` commands
```

```yml
Command:
```
# load

```bash
@jaseci > help load
Usage: load [OPTIONS] COMMAND [ARGS]...

  Group of `load` commands

Options:
  --help  Show this message and exit.

Commands:
  yaml  applying list of yaml files without associating to any...
```

```yml
Command:
```
# logger

```bash
@jaseci > help logger
Usage: logger [OPTIONS] COMMAND [ARGS]...

  Group of `logger` commands

Options:
  --help  Show this message and exit.

Commands:
  get   Get logs across loggers
  http  Group of `logger http` commands
  list  Check active loggers
```

```yml
Command:
```
# login

```bash
@jaseci > help login
Usage: login [OPTIONS] URL

  Command to log into live Jaseci server

Options:
  -u, --username TEXT  Username to be used for login.  [required]
  --password TEXT      Password to be used for login.
  --help               Show this message and exit.
```

```yml
Command:
```
# logout 

```bash
@jaseci > help logout
Usage: logout [OPTIONS]

  Command to log out of live Jaseci server

Options:
  --help  Show this message and exit.
```

```yml
Command:
```
# ls 

```bash
@jaseci > help ls
Usage: ls [OPTIONS]

  List relevant files

Options:
  -a, --all  Flag for listing all files, not just relevant files
  --help     Show this message and exit.
```

```yml
Command:
```
# master

```bash
@jaseci > help master
Usage: master [OPTIONS] COMMAND [ARGS]...

  Group of `master` commands

Options:
  --help  Show this message and exit.

Commands:
  active       Group of `master active` commands
  allusers     Returns info on a set of users, limit specifies the number...
  become       Sets the default master master should use
  create       Create a master instance and return root node master object
  createsuper  Create a super instance and return root node super object
  delete       Permanently delete master with given id
  get          Return the content of the master with mode Valid modes:...
  list         Provide complete list of all master objects (list of root...
  self         Returns the masters object
  unbecome     Unsets the default master master should use
```

```yml
Command:
```
# object

```bash
@jaseci > help object
Usage: object [OPTIONS] COMMAND [ARGS]...

  Group of `object` commands

Options:
  --help  Show this message and exit.

Commands:
  get    Returns object details for any Jaseci object.
  perms  Group of `object perms` commands
```

```yml
Command:
```
# prometheus

```bash
@jaseci > help prometheus
Usage: prometheus [OPTIONS] COMMAND [ARGS]...

  Group of `prometheus` commands

Options:
  --help  Show this message and exit.

Commands:
  metrics  Group of `prometheus metrics` commands
  node     Group of `prometheus node` commands
  pod      Group of `prometheus pod` commands
```

```yml
Command:
```
# publogin

```bash
@jaseci > help publogin
Usage: publogin [OPTIONS] URL

  Command for unauthenticated log into live Jaseci server

Options:
  --help  Show this message and exit.
```

```yml
Command:
```
# reset

```bash
@jaseci > help reset
Usage: reset [OPTIONS]

  Reset jsctl (clears state)

Options:
  --help  Show this message and exit.
```

```yml
Command:
```
# script

```bash
@jaseci > help script
Usage: script [OPTIONS] FILENAME

  Run multiple commands sequentially from file

Options:
  -p, --profile
  -o, --output TEXT  Filename to dump output of this command call.
  --help             Show this message and exit.
```

```yml
Command:
```
# sentinel

```bash
@jaseci > help sentinel
Usage: sentinel [OPTIONS] COMMAND [ARGS]...

  Group of `sentinel` commands

Options:
  --help  Show this message and exit.

Commands:
  active    Group of `sentinel active` commands
  delete    Permanently delete sentinel with given id
  get       Get a sentinel rendered with specific mode Valid modes:...
  list      Provide complete list of all sentinel objects
  pull      Copies global sentinel to local master
  register  Create blank or code loaded sentinel and return object...
  set       Set code/ir for a sentinel, only replaces walkers/archs in...
  test      Run battery of test cases within sentinel and provide result
```

```yml
Command:
```
# service

```bash
@jaseci > help service
Usage: service [OPTIONS] COMMAND [ARGS]...

  Group of `service` commands

Options:
  --help  Show this message and exit.

Commands:
  call     temporary api for retreiving/calling attributes of specific...
  refresh  refreshing service's config.
```

```yml
Command:
```
# user

```bash
@jaseci > help user
Usage: user [OPTIONS] COMMAND [ARGS]...

  Group of `user` commands

Options:
  --help  Show this message and exit.

Commands:
  create      Create a new user (master object)
  delete      Delete new user (master object)
  deleteself  Delete self (master object)
```

```yml
Command:
```
# walker

```bash
@jaseci > help walker
Usage: walker [OPTIONS] COMMAND [ARGS]...

  Group of `walker` commands

Options:
  --help  Show this message and exit.

Commands:
  callback  Public api for running walkers, namespace key must be...
  execute   Executes walker (assumes walker is primed)
  get       Get a walker rendered with specific mode Valid modes:...
  list      List walkers known to sentinel
  prime     Assigns walker to a graph node and primes walker for execution
  queue     Group of `walker queue` commands
  run       Creates walker instance, primes walker on node, executes...
  spawn     Group of `walker spawn` commands
  step      Executes walker (assumes walker is primed)
  summon    Public api for running walkers, namespace key must be...
  total     Get total walkers known to sentinel
  yield     Group of `walker yield` commands
```

```yml
Command:
```
# wapi

```bash
@jaseci > help wapi
Usage: wapi [OPTIONS] NAME

  Walker individual APIs

Options:
  -o, --output TEXT   Filename to dump output of this command call.
  -profiling BOOLEAN
  -snt TEXT
  -_req_ctx TEXT
  -ctx TEXT
  -nd TEXT
  --help              Show this message and exit.
```


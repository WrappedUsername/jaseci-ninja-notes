# [Jaseci](https://docs.jaseci.org/) Ninja Notes - 🚧 Work In Progress 🏗

- *These are only my notes, not official docs here, official docs are found in the link provided above*

<p align="left"> 
<img src="https://komarev.com/ghpvc/?username=jaseci-ninja-notes&label=Profile%20views&color=f79952&style=flat" alt="jaseci-ninja-notes" /> 
<img alt="Stars" src="https://img.shields.io/github/stars/WrappedUsername/jaseci-ninja-notes?style=flat-square&labelColor=343b41"/>
</p>

## My notes from learning Jaseci runtime and Jac programming language

```yml
Saving state with a maintainer walker:
```

```jac
can cleanup with talker entry{
    if (!vistor:hoping) {
       spawn *(global.node_conv_root_state) walker::maintainer(
            user_id = visitor.user_id,
            user_context = vistor.user_context,
            dialogue_context = vistor.dialogue_context,
            last_conv_state = vistor.state_for_continuing
            // Add ERC-4337 account abstractions or any other saved states, etc here.
       );
    }
}
```

[reference: Jaseci Bible](https://github.com/Jaseci-Labs/jaseci/raw/main/support/bible/pdf/jaseci_bible.pdf)

```yml
Jaseci Graph described as a 7-tuple (N, E, C, s, t, cN , cE ), where:
```

```mermaid
---
title: 7-tuple (N, E, C, s, t, cN , cE) Jaseci Graph
---
classDiagram
  N --> E : s = source 
  N --> E : t = target
  cN <-- N : cN = nodes to context
  cE <-- E : cE = edges to context
  class N{
    +nodes in graph
  }
  class E{
    +edges in graph
  }
  class C{
    +set of all contexts
  }
```

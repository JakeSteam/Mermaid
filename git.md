# Git graphs cheatsheet

[Official documentation](https://mermaid.js.org/syntax/gitgraph.html).

## Basic graph

```mermaid
gitGraph:
    commit
    commit
    commit
```

```
gitGraph:
    commit
    commit
    commit
```

## Branching, checking out, and merging

```mermaid
gitGraph:
    commit
    branch branch2
    checkout branch2
    commit
    checkout main
    commit
    merge branch2
```

```
gitGraph:
    commit
    branch branch2
    checkout branch2
    commit
    checkout main
    commit
    merge branch2
```

## Notes

- There is no official documentation yet for git graphs.
- The git commits seem to change frequently, and cannot be specified.

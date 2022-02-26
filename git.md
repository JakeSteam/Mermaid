# Git graphs cheatsheet

[Live editor](https://mermaid-js.github.io/mermaid-live-editor/edit#pako:eNplj7EOwjAMRH-l8twBBpbMIHZYvZjEtBHEqVJHCFX9d0JLURFebN09WXcD2OgYDDRej4m61qDETn2UHmVAqcogSGHOHVkvDYKptrtNvbZO5HzuJ2eDMqKwOBQbQ_CKckkktq2EH_NVnJbtLWb90T70dy9MoF45_QOBU8PrD1BD0QJ5V-pM0RG05cDvYAiOr5TvilASFjR3jpQPzmtMYK5077kGyhrPT7FgNGVeoL2nJlGYxfEF4jtu2A).

## Graph direction

```mermaid
gitGraph LR:
    checkout master
    commit
    commit
    commit
```

```
gitGraph LR:
    checkout master
    commit
    commit
    commit
```

```mermaid
gitGraph BT:
    checkout master
    commit
    commit
    commit
```

```
gitGraph BT:
    checkout master
    commit
    commit
    commit
```

## Commit messages

```mermaid
gitGraph BT:
    checkout master
    commit "Commit message"
    commit "Another message"
    commit "Yet another message"
```

```
gitGraph BT:
    checkout master
    commit "Commit message"
    commit "Another message"
    commit "Yet another message"
```

## Branching, checking out, and merging

```mermaid
gitGraph BT:
    commit
    branch branch2
    checkout branch2
    commit
    checkout master
    commit
    merge branch2
```

```
gitGraph BT:
    commit
    branch branch2
    checkout branch2
    commit
    checkout master
    commit
    merge branch2
```

## Notes

* There is no official documentation yet for git graphs.
* The git commits seem to change frequently, and cannot be specified.
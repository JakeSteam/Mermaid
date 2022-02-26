# State diagrams cheatsheet

[Official documentation](https://mermaid-js.github.io/mermaid/#/stateDiagram) & [live editor](https://mermaid-js.github.io/mermaid-live-editor/#/edit/eyJjb2RlIjoic3RhdGVEaWFncmFtLXYyXG4gICAgWypdIC0tPiBTdGlsbFxuICAgIFN0aWxsIC0tPiBbKl1cbiAgICBTdGlsbCAtLT4gTW92aW5nXG4gICAgTW92aW5nIC0tPiBTdGlsbFxuICAgIE1vdmluZyAtLT4gQ3Jhc2hcbiAgICBDcmFzaCAtLT4gWypdIiwibWVybWFpZCI6eyJ0aGVtZSI6ImRlZmF1bHQiLCJ0aGVtZVZhcmlhYmxlcyI6eyJiYWNrZ3JvdW5kIjoid2hpdGUiLCJwcmltYXJ5Q29sb3IiOiIjRUNFQ0ZGIiwic2Vjb25kYXJ5Q29sb3IiOiIjZmZmZmRlIiwidGVydGlhcnlDb2xvciI6ImhzbCg4MCwgMTAwJSwgOTYuMjc0NTA5ODAzOSUpIiwicHJpbWFyeUJvcmRlckNvbG9yIjoiaHNsKDI0MCwgNjAlLCA4Ni4yNzQ1MDk4MDM5JSkiLCJzZWNvbmRhcnlCb3JkZXJDb2xvciI6ImhzbCg2MCwgNjAlLCA4My41Mjk0MTE3NjQ3JSkiLCJ0ZXJ0aWFyeUJvcmRlckNvbG9yIjoiaHNsKDgwLCA2MCUsIDg2LjI3NDUwOTgwMzklKSIsInByaW1hcnlUZXh0Q29sb3IiOiIjMTMxMzAwIiwic2Vjb25kYXJ5VGV4dENvbG9yIjoiIzAwMDAyMSIsInRlcnRpYXJ5VGV4dENvbG9yIjoicmdiKDkuNTAwMDAwMDAwMSwgOS41MDAwMDAwMDAxLCA5LjUwMDAwMDAwMDEpIiwibGluZUNvbG9yIjoiIzMzMzMzMyIsInRleHRDb2xvciI6IiMzMzMiLCJtYWluQmtnIjoiI0VDRUNGRiIsInNlY29uZEJrZyI6IiNmZmZmZGUiLCJib3JkZXIxIjoiIzkzNzBEQiIsImJvcmRlcjIiOiIjYWFhYTMzIiwiYXJyb3doZWFkQ29sb3IiOiIjMzMzMzMzIiwiZm9udEZhbWlseSI6IlwidHJlYnVjaGV0IG1zXCIsIHZlcmRhbmEsIGFyaWFsIiwiZm9udFNpemUiOiIxNnB4IiwibGFiZWxCYWNrZ3JvdW5kIjoiI2U4ZThlOCIsIm5vZGVCa2ciOiIjRUNFQ0ZGIiwibm9kZUJvcmRlciI6IiM5MzcwREIiLCJjbHVzdGVyQmtnIjoiI2ZmZmZkZSIsImNsdXN0ZXJCb3JkZXIiOiIjYWFhYTMzIiwiZGVmYXVsdExpbmtDb2xvciI6IiMzMzMzMzMiLCJ0aXRsZUNvbG9yIjoiIzMzMyIsImVkZ2VMYWJlbEJhY2tncm91bmQiOiIjZThlOGU4IiwiYWN0b3JCb3JkZXIiOiJoc2woMjU5LjYyNjE2ODIyNDMsIDU5Ljc3NjUzNjMxMjglLCA4Ny45MDE5NjA3ODQzJSkiLCJhY3RvckJrZyI6IiNFQ0VDRkYiLCJhY3RvclRleHRDb2xvciI6ImJsYWNrIiwiYWN0b3JMaW5lQ29sb3IiOiJncmV5Iiwic2lnbmFsQ29sb3IiOiIjMzMzIiwic2lnbmFsVGV4dENvbG9yIjoiIzMzMyIsImxhYmVsQm94QmtnQ29sb3IiOiIjRUNFQ0ZGIiwibGFiZWxCb3hCb3JkZXJDb2xvciI6ImhzbCgyNTkuNjI2MTY4MjI0MywgNTkuNzc2NTM2MzEyOCUsIDg3LjkwMTk2MDc4NDMlKSIsImxhYmVsVGV4dENvbG9yIjoiYmxhY2siLCJsb29wVGV4dENvbG9yIjoiYmxhY2siLCJub3RlQm9yZGVyQ29sb3IiOiIjYWFhYTMzIiwibm90ZUJrZ0NvbG9yIjoiI2ZmZjVhZCIsIm5vdGVUZXh0Q29sb3IiOiJibGFjayIsImFjdGl2YXRpb25Cb3JkZXJDb2xvciI6IiM2NjYiLCJhY3RpdmF0aW9uQmtnQ29sb3IiOiIjZjRmNGY0Iiwic2VxdWVuY2VOdW1iZXJDb2xvciI6IndoaXRlIiwic2VjdGlvbkJrZ0NvbG9yIjoicmdiYSgxMDIsIDEwMiwgMjU1LCAwLjQ5KSIsImFsdFNlY3Rpb25Ca2dDb2xvciI6IndoaXRlIiwic2VjdGlvbkJrZ0NvbG9yMiI6IiNmZmY0MDAiLCJ0YXNrQm9yZGVyQ29sb3IiOiIjNTM0ZmJjIiwidGFza0JrZ0NvbG9yIjoiIzhhOTBkZCIsInRhc2tUZXh0TGlnaHRDb2xvciI6IndoaXRlIiwidGFza1RleHRDb2xvciI6IndoaXRlIiwidGFza1RleHREYXJrQ29sb3IiOiJibGFjayIsInRhc2tUZXh0T3V0c2lkZUNvbG9yIjoiYmxhY2siLCJ0YXNrVGV4dENsaWNrYWJsZUNvbG9yIjoiIzAwMzE2MyIsImFjdGl2ZVRhc2tCb3JkZXJDb2xvciI6IiM1MzRmYmMiLCJhY3RpdmVUYXNrQmtnQ29sb3IiOiIjYmZjN2ZmIiwiZ3JpZENvbG9yIjoibGlnaHRncmV5IiwiZG9uZVRhc2tCa2dDb2xvciI6ImxpZ2h0Z3JleSIsImRvbmVUYXNrQm9yZGVyQ29sb3IiOiJncmV5IiwiY3JpdEJvcmRlckNvbG9yIjoiI2ZmODg4OCIsImNyaXRCa2dDb2xvciI6InJlZCIsInRvZGF5TGluZUNvbG9yIjoicmVkIiwibGFiZWxDb2xvciI6ImJsYWNrIiwiZXJyb3JCa2dDb2xvciI6IiM1NTIyMjIiLCJlcnJvclRleHRDb2xvciI6IiM1NTIyMjIiLCJjbGFzc1RleHQiOiIjMTMxMzAwIiwiZmlsbFR5cGUwIjoiI0VDRUNGRiIsImZpbGxUeXBlMSI6IiNmZmZmZGUiLCJmaWxsVHlwZTIiOiJoc2woMzA0LCAxMDAlLCA5Ni4yNzQ1MDk4MDM5JSkiLCJmaWxsVHlwZTMiOiJoc2woMTI0LCAxMDAlLCA5My41Mjk0MTE3NjQ3JSkiLCJmaWxsVHlwZTQiOiJoc2woMTc2LCAxMDAlLCA5Ni4yNzQ1MDk4MDM5JSkiLCJmaWxsVHlwZTUiOiJoc2woLTQsIDEwMCUsIDkzLjUyOTQxMTc2NDclKSIsImZpbGxUeXBlNiI6ImhzbCg4LCAxMDAlLCA5Ni4yNzQ1MDk4MDM5JSkiLCJmaWxsVHlwZTciOiJoc2woMTg4LCAxMDAlLCA5My41Mjk0MTE3NjQ3JSkifX0sInVwZGF0ZUVkaXRvciI6ZmFsc2V9).

## Essentials

### Basic syntax

```mermaid
stateDiagram-v2
    direction LR
    s1 : State with description

    [*] --> SimpleState: Transition text
    SimpleState --> s1: Also transition text
    s1 --> [*]
```

```
stateDiagram-v2
    direction LR
    s1 : State with description

    [*] --> SimpleState: Transition text
    SimpleState --> s1: Also transition text
    s1 --> [*]
```

### Direction

```mermaid
stateDiagram-v2
    direction TB
    state Left-to-right {
        direction LR
        a --> b
    }
    state Right-to-left {
        direction RL
        c --> d
    }
    state Top-to-bottom {
        direction TB
        e --> f
    }
    state Bottom-to-top {
        direction BT
        g --> h
    }
```

```
stateDiagram-v2
    direction TB
    state Left-to-right {
        direction LR
        a --> b
    }
    state Right-to-left {
        direction RL
        c --> d
    }
    state Top-to-bottom {
        direction TB
        e --> f
    }
    state Bottom-to-top {
        direction BT
        g --> h
    }
```

## Connecting states

### Simple

```mermaid
stateDiagram-v2
    direction LR
    [*] --> Ready
    Ready --> Moving
    Moving --> Ready
    Moving --> Zooming
    Moving --> Crashed
    Zooming --> Zoooooming
    Zoooooming --> Crashed
    Crashed --> [*]
```

```
stateDiagram-v2
    direction LR
    [*] --> Ready
    Ready --> Moving
    Moving --> Ready
    Moving --> Zooming
    Moving --> Crashed
    Zooming --> Zoooooming
    Zoooooming --> Crashed
    Crashed --> [*]
```

### Conditional (choice)

```mermaid
stateDiagram-v2
    state BigOrSmall <<choice>>
    Start --> BigOrSmall
    BigOrSmall --> Big : It's a big number!
    BigOrSmall --> Or: It's not a number at all..!
    BigOrSmall --> Small : It's a small number!
```

```
stateDiagram-v2
    state BigOrSmall <<choice>>
    Start --> BigOrSmall
    BigOrSmall --> Big : It's a big number!
    BigOrSmall --> Or: It's not a number at all..!
    BigOrSmall --> Small : It's a small number!
```

### Splits (fork / join)

```mermaid
stateDiagram-v2
    state BigOrSmall <<fork>>
    state DoesntMatter <<join>>
    Start --> BigOrSmall
    BigOrSmall --> Big : It's a big number!
    BigOrSmall --> Or: It's not a number at all..!
    BigOrSmall --> Small : It's a small number!
    Big --> DoesntMatter
    Or --> DoesntMatter
    Small --> DoesntMatter  
```

```
stateDiagram-v2
    state BigOrSmall <<fork>>
    state DoesntMatter <<join>>
    Start --> BigOrSmall
    BigOrSmall --> Big : It's a big number!
    BigOrSmall --> Or: It's not a number at all..!
    BigOrSmall --> Small : It's a small number!
    Big --> DoesntMatter
    Or --> DoesntMatter
    Small --> DoesntMatter  
```

## Subdiagrams

### Multiple state diagrams

```mermaid
stateDiagram-v2
    First --> Second
    First --> Third

    state First {
        a --> b
    }
    state Second {
        c --> d
    }
    state Third {
        e --> f
    }
```

```
stateDiagram-v2
    First --> Second
    First --> Third

    state First {
        a --> b
    }
    state Second {
        c --> d
    }
    state Third {
        e --> f
    }
```

### Nested state diagrams

```mermaid
stateDiagram-v2

    state First {
        direction LR
        a --> Second
    }
    state Second {
        direction LR
        b --> Third
    }
    state Third {
        direction LR
        c --> d
    }
```

```
stateDiagram-v2

    state First {
        direction LR
        a --> Second
    }
    state Second {
        direction LR
        b --> Third
    }
    state Third {
        direction LR
        c --> d
    }
```

### Concurrency

```mermaid
stateDiagram-v2

    state BackpackOpen {
        TorchOn --> TorchOff : Turn torch on
        TorchOff --> TorchOn : Turn torch off
        --
        EatingCandy --> GettingCandy : Finished candy
        GettingCandy --> EatingCandy : Started candy
        --
        PhoneOn --> PhoneOff : Turn phone on
        PhoneOff --> PhoneOn : Turn phone off
    }
```

```
stateDiagram-v2

    state BackpackOpen {
        TorchOn --> TorchOff : Turn torch on
        TorchOff --> TorchOn : Turn torch off
        --
        EatingCandy --> GettingCandy : Finished candy
        GettingCandy --> EatingCandy : Started candy
        --
        PhoneOn --> PhoneOff : Turn phone on
        PhoneOff --> PhoneOn : Turn phone off
    }
```

## Other

### Notes

```mermaid
stateDiagram-v2
    direction LR
    Start --> Middle
    Middle --> End

    note left of Start
        "left" makes a left note in left-to-right, 
        and a top note in top-to-bottom.
    end note

    note right of Start
        "right" makes a right note in left-to-right, 
        and a bottom note in top-to-bottom.
    end note
```

```
stateDiagram-v2
    direction LR
    Start --> Middle
    Middle --> End

    note left of Start
        "left" makes a left note in left-to-right, 
        and a top note in top-to-bottom.
    end note

    note right of Start
        "right" makes a right note in left-to-right, 
        and a bottom note in top-to-bottom.
    end note
```

### Comments

```mermaid
stateDiagram-v2
    direction LR
    First --> Second %% Here's a comment
    Second --> Third
    %% Here's another comment
```

```
stateDiagram-v2
    direction LR
    First --> Second %% Here's a comment
    Second --> Third
    %% Here's another comment
```
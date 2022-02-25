# State diagrams

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

### Conditional (choice)

```mermaid
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

### Comments

```mermaid
stateDiagram-v2
    direction LR
    First --> Second %% Here's a comment
    Second --> Third
    %% Here's another comment

```
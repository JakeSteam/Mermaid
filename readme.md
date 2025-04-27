> [!WARNING]  
> This PR reflects Mermaid syntax as of ~2022, and doesn't include newer diagram types (yet). Feel free to raise a PR adding them!

# Mermaid syntax references

A rewrite of [the Mermaid documentation](https://mermaid.js.org/intro/syntax-reference.html) as a learning aid and cheatsheet.

<table>
<tr><td>Example</td><td>Code</td></tr>

<tr><td>

```mermaid
flowchart LR
    A[Start] --> B{Should you?}
    B -- Yes --> C{{Do it}}
    B -- Maybe --> D[(Save for later)]
    B -- No --> E[Okay]
```

</td><td>

```
flowchart LR
    A[Start] --> B{Should you?}
    B -- Yes --> C{{Do it}}
    B -- Maybe --> D[(Save for later)]
    B -- No --> E[Okay]
```

<a href="/flowchart.md">Flowchart in Mermaid cheatsheet</a>

</td></tr>
<tr><td>

```mermaid
sequenceDiagram
    Alice ->>+ Bob: Here's a message!
    Bob ->>- Alice: Hmm, ok, thanks.
```

</td><td>

```
sequenceDiagram
    Alice ->>+ Bob: Here's a message!
    Bob ->>- Alice: Hmm, ok, thanks.
```

<a href="/sequence.md">Sequence diagram in Mermaid cheatsheet</a>

</td></tr>
<tr><td>

```mermaid
classDiagram
    class ClassName {
        String stringName
        Long longName
        MyDatatype attributeName

        functionName(parameter) ReturnType
        functionName2(parameter2) ReturnType
    }
    class Interface {
        Int intName
    }
    ClassName --|> Interface
```

</td><td>

```
classDiagram
    class ClassName {
        String stringName
        Long longName
        MyDatatype attributeName

        functionName(parameter) ReturnType
        functionName2(parameter2) ReturnType
    }
    class Interface {
        Int intName
    }
    ClassName --|> Interface
```

<a href="/class.md">Class diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
stateDiagram-v2
    Stationary --> Moving : Begin moving
    Moving --> Stationary : Stop moving
```

</td><td>

```
stateDiagram-v2
    Stationary --> Moving : Begin moving
    Moving --> Stationary : Stop moving
```

<a href="/state.md">State diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
erDiagram
    User {
        Int id PK
        String username
        Int serverId FK
    }

    Server {
        Int id PK
        String serverName
    }

    Server ||--o{ User : has
```

</td><td>

```
erDiagram
    User {
        Int id PK
        String username
        Int serverId FK
    }

    Server {
        Int id PK
        String serverName
    }

    Server ||--o{ User : has
```

<a href="/entity-relationship.md">Entity relationship diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
journey
    title User Journey
    section Logging in
        Navigate to login: 4: Alice, Bob, Craig
        Entering details: 2: Alice, Bob
        Pressing button: 5: Alice
```

</td><td>

```
journey
    title User Journey
    section Logging in
        Navigate to login: 4: Alice, Bob, Craig
        Entering details: 2: Alice, Bob
        Pressing button: 5: Alice
```

<a href="/user-journey.md">User journey diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
gantt
    Dated Milestone: milestone, m1, 2023-01-01, 1d
    Relative Milestone: milestone, m2, after m1, 1d
    Task 1: a1, 2023-01-01, 1d
    Task 2: a2, after a1, 1d
    Task 3: a3, 2023-01-01, 36hr
```

</td><td>

```
gantt
    Dated Milestone: milestone, m1, 2023-01-01, 1d
    Relative Milestone: milestone, m2, after m1, 1d
    Task 1: a1, 2023-01-01, 1d
    Task 2: a2, after a1, 1d
    Task 3: a3, 2023-01-01, 36hr
```

<a href="/gantt.md">Gantt chart in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
pie
    title Fruits
    "Apples" : 50
    "Oranges" : 20
    "Grapes" : 9.99
    "Passionfruits" : 12.5
```

</td><td>

```
pie
    title Fruits
    "Apples" : 50
    "Oranges" : 20
    "Grapes" : 9.99
    "Passionfruits" : 12.5
```

<a href="/pie.md">Pie chart in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
quadrantChart
    title Title of quadrant chart
    x-axis X low value --> X high value
    y-axis Y low value --> Y high value
    quadrant-1 Top right name
    quadrant-2 Top left name
    quadrant-3 Bottom left name
    quadrant-4 Bottom right name
    Value A: [0.1, 0.2]
    Value B: [0.9, 0.8]
    Value C: [0.5, 0.5]
    Value D: [0.9, 0.9]
```

</td><td>

```
quadrantChart
    title Title of quadrant chart
    x-axis X low value --> X high value
    y-axis Y low value --> Y high value
    quadrant-1 Top right name
    quadrant-2 Top left name
    quadrant-3 Bottom left name
    quadrant-4 Bottom right name
    Value A: [0.1, 0.2]
    Value B: [0.9, 0.8]
    Value C: [0.5, 0.5]
    Value D: [0.9, 0.9]
```

<a href="/quadrant.md">Quadrant diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
    requirementDiagram

    requirement UptimeRequirement {
        id: 1
        text: Site Uptime
        risk: Medium
        verifymethod: Analysis
    }

    element satisfyingElement {
        type: MyElement
        docref: ABC001
    }

    element containingElement {
        type: MyElement
        docref: ABC002
    }

    satisfyingElement - satisfies -> UptimeRequirement
    containingElement - contains -> UptimeRequirement
```

</td><td>

```
    requirementDiagram

    requirement UptimeRequirement {
        id: 1
        text: Site Uptime
        risk: Medium
        verifymethod: Analysis
    }

    element satisfyingElement {
        type: MyElement
        docref: ABC001
    }

    element containingElement {
        type: MyElement
        docref: ABC002
    }

    satisfyingElement - satisfies -> UptimeRequirement
    containingElement - contains -> UptimeRequirement
```

<a href="/requirement.md">Requirement diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

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

</td><td>

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

<a href="/git.md">Git graphs in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
    C4
```

</td><td>

```
    C4
```

<a href="/c4.md">C4 diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
    mindmaps
```

</td><td>

```
    mindmaps
```

<a href="/mindmaps.md">Mindmaps diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
    timeline
```

</td><td>

```
    timeline
```

<a href="/timeline.md">Timeline diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
    zenUML
```

</td><td>

```
    zenUML
```

<a href="/zenuml.md">ZenUML diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
    sankey
```

</td><td>

```
    sankey
```

<a href="/sankey.md">Sankey diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
    XY
```

</td><td>

```
    XY
```

<a href="/xy.md">XY diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
    block
```

</td><td>

```
    block
```

<a href="/block.md">Block diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
    packet
```

</td><td>

```
    packet
```

<a href="/packet.md">Packet diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
    kanban
```

</td><td>

```
    kanban
```

<a href="/kanban.md">Kanban diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
    architecture
```

</td><td>

```
    architecture
```

<a href="/architecture.md">Architecture diagram in Mermaid cheatsheet</a></td></tr>

<tr><td>

```mermaid
    radar
```

</td><td>

```
    radar
```

<a href="/radar.md">Radar diagram in Mermaid cheatsheet</a></td></tr>

</table>

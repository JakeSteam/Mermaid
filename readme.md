# Mermaid syntax references

A concise rewrite of [the mermaid documentation](https://mermaid-js.github.io/mermaid/) for quick lookups.

Meta:
* Overview (comments, configuring, etc)

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

<a href="/1-flowchart.md">Flowchart cheatsheet</a>
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

<a href="/2-sequence.md">Sequence diagram cheatsheet</a>
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
<a href="/3-class.md">Class diagram cheatsheet</a></td></tr>
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

<a href="/4-state.md">State diagram cheatsheet</a></td></tr>
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
<a href="/5-entity-relationship.md">Entity relationship diagram cheatsheet</a></td></tr>
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

<a href="/6-user-journey.md">User journey diagram cheatsheet</a></td></tr>
<tr><td>

```mermaid
gantt
    Dated Milestone: milestone, m1, today, 1d
    Relative Milestone: milestone, m2, after m1, 1d
    Task 1: a1, today, 1d
    Task 2: a2, after a1, 1d
    Task 3: a3, today, 36hr
```

</td><td>

```
gantt
    Dated Milestone: milestone, m1, today, 1d
    Relative Milestone: milestone, m2, after m1, 1d
    Task 1: a1, today, 1d
    Task 2: a2, after a1, 1d
    Task 3: a3, today, 36hr
```

<a href="/7-gantt.md">Gantt chart cheatsheet</a></td></tr>
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

<a href="/8-pie.md">Pie chart cheatsheet</a></td></tr>
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

<a href="/9-requirement">Requirement diagram cheatsheet</a></td></tr>

</table>
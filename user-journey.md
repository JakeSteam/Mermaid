# User journey diagrams cheatsheet

[Official documentation](https://mermaid-js.github.io/mermaid/#/user-journey) & [live editor](https://mermaidjs.github.io/mermaid-live-editor/#/edit/eyJjb2RlIjoic3RhdGVEaWFncmFtXG4gICAgWypdIC0tPiBTdGlsbFxuICAgIFN0aWxsIC0tPiBbKl1cbiAgICBTdGlsbCAtLT4gTW92aW5nXG4gICAgTW92aW5nIC0tPiBTdGlsbFxuICAgIE1vdmluZyAtLT4gQ3Jhc2hcbiAgICBDcmFzaCAtLT4gWypdIiwibWVybWFpZCI6eyJ0aGVtZSI6ImRlZmF1bHQifX0).

## Defining sections and tasks

```mermaid
journey
    title Sections and Tasks
    section Section One
        Task inside Section One: 5 
    section Section Two
        Task inside Section Two: 5
        Task2 inside Section Two: 5
    section Section Three
        Task inside Section Three: 5
        Task2 inside Section Three: 5
        Task3 inside Section Three: 5
```

```
journey
    title Sections and Tasks
    section Section One
        Task inside Section One: 5 
    section Section Two
        Task inside Section Two: 5
        Task2 inside Section Two: 5
    section Section Three
        Task inside Section Three: 5
        Task2 inside Section Three: 5
        Task3 inside Section Three: 5
```

## Defining users

```mermaid
journey
    title Users
    section Section One
        Task 1: 5: User1, User2, User3, User4, User5
        Task 2: 5: User1, User2, User99
        Task 3: 5
        Task 4: 5: User99
```

```
journey
    title Users
    section Section One
        Task 1: 5: User1, User2, User3, User4, User5
        Task 2: 5: User1, User2, User99
        Task 3: 5
        Task 4: 5: User99
```

## Defining score

```mermaid
journey
    title Score
    section Section 1
        Score 0/5: 0
        Score 1/5: 1
        Score 2/5: 2
        Score 3/5: 3
        Score 4/5: 4
        Score 5/5: 5
        Score N/A/5: X
```

```
journey
    title Score
    section Section 1
        Score 0/5: 0
        Score 1/5: 1
        Score 2/5: 2
        Score 3/5: 3
        Score 4/5: 4
        Score 5/5: 5
        Score N/A/5: X
```
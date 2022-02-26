# Gantt chart

```mermaid
gantt
    title Planning
    section First Section
        First 30d task : a1, 2020-01-01, 30d
        Next 7d task : a2, after a1, 7d
    section Second Section
        Next task : a3, 2020-02-01, 12d
        Final task : 24d
```

## Defining

### Defining tasks

```mermaid
gantt
    Dated task: task1, 2020-01-01, 7d
    Subsequent task: task3, after task1, 7d
    Critical task: crit, task5, 2020-01-01, 8d
    Active task: active, task6, 2020-01-01, 6d
    Done task: done, task7, 2020-01-01, 5d
    Critical active task: crit, active, 2020-01-01, 6d
    Critical done task: crit, done, 2020-01-01, 6d
    Task after multiple tasks: task4, after task5 task6 task7, 4d
```

### Defining sections

```mermaid
gantt
    Task with no section: a1, 2020-01-01, 25d
    section First Section
        A Task: a2, 2020-01-01, 7d
        Another task: a3, after a2, 7d
    section Second Section
        Next task: a4, 2020-01-12, 10d
        Final task: 5d
```

### Defining milestones & daily marker

```mermaid
gantt
    todayMarker stroke-width:5px,stroke:#0f0,opacity:0.5
    %% or `todayMarker off`
    Dated Milestone: milestone, m1, today, 3d
    Relative Milestone: milestone, m2, after m1, 5d
    Task 1: a1, today, 3d
    Task 2: a2, after a1, 5d
```

## Configuring

### Configuring date format

`dateFormat` defines the **input** date format (i.e. the format datetimes are defined in).

`axisFormat` defines the **output** date format (i.e. the format shown on the x axis).

Both have different placeholder values, see [official documentation](https://mermaid-js.github.io/mermaid/#/gantt?id=setting-dates).

```mermaid
gantt
    dateFormat HH:mm
    axisFormat %H:%M
    First Milestone: milestone, m1, 03:20, 0m
    Second Milestone: milestone, m2, 07:00, 1m
    Task 1: a1, 02:45, 2h
    Task 2: a2, after a1, 2h
```

### Configuring title

```mermaid
gantt
    title The Chart's Title
    Task 1: a1, 2020-01-01, 3d
    Task 2: a2, after a1, 5d
```

## Other

### Comments

```mermaid
gantt
    %% Comments can go here
    section Main Section
        %% Or here
        Task 1: a1, 2020-01-01, 3d
        Task 2: a2, after a1, 5d
```

### Links

```mermaid
gantt
    Clickable link 1: a1, 2020-01-01, 3d
    Clickable link 2: a2, after a1, 5d
    click a1 href "https://example.com"
    click a2 call "https://example.com/2"
```

JavaScript click events can also be triggered, see [official documentation](https://mermaid-js.github.io/mermaid/#/gantt?id=interaction).
### Styling

Styling is performed with CSS, see [official documentation](https://mermaid-js.github.io/mermaid/#/gantt?id=styling).
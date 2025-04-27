# Timeline charts cheatsheet

[Official documentation](https://mermaid.js.org/syntax/timeline.html).

## Basic syntax

```mermaid
timeline
    title Timeline title
    2001: Something happened
    2002: Something else happened
    2003: Another thing happened
    Whenever: This happened!
            : And this!
```

```
timeline
    title Timeline title
    2001: Something happened
    2002: Something else happened
    2003: Another thing happened
    Whenever: This happened!
            : And this!
```

## Grouping

```mermaid
timeline
    title Timeline title
    section 2000
        January: Event 1
        March: Event 2
        April: Event 3
    section 2001
    section 2002
        June: Event 4
    section Future
```

```
timeline
    title Timeline title
    2001: Something happened
    2002: Something else happened
    2003: Another thing happened
    Whenever: This happened!
            : And this!
```

## Styling

The individual elements can be styled, but this must be done [on Mermaid initialization](https://mermaid.js.org/syntax/timeline.html#styling-of-time-periods-and-events), or by [setting a theme](https://mermaid.js.org/syntax/timeline.html#themes).

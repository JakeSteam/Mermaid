# Requirement diagrams cheatsheet

[Official documentation](https://mermaid-js.github.io/mermaid/#/requirementDiagram).

## Defining requirements

```mermaid
requirementDiagram
    requirement UptimeRequirement {
        id: 1
        text: Site Uptime 
        risk: Medium
        verifymethod: Analysis
    }
```

* `requirement` can be replaced by `functionalRequirement`, `interfaceRequirement`, `performanceRequirement`, `physicalRequirement`, or `designConstraint`.
* `risk` can be defined as `Low`, `Medium`, or `High`.
* `verifyMethod` can be defined as `Analysis`, `Inspection`, `Test`, or `Demonstration`.

## Defining elements

```mermaid
requirementDiagram
    element myEntity {
        type: MyElement
        docref: ABC123
    }
```

## Defining relationships

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

* `satisfies` can be replaced by `contains`, `copies`, `derives`, `verifies`, `refines`, or `traces`.
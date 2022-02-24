# Flowcharts

## Chart Orientation

<table>
    <tr><td></td><td>Standard</td><td>Reversed</td></tr>
    <tr><td>Vertical</td>
<td>

```mermaid
flowchart TB; 
    Start --> Middle --> End
```
**TB**: Top to Bottom<br>(also **TD**: Top down)

</td>
<td>

```mermaid
flowchart BT; 
    Start --> Middle --> End
```
**BT**: Bottom to Top

</td>
    </tr>
    <tr><td>Horizontal</td>
<td>

```mermaid
flowchart LR; 
    Start --> Middle --> End
```
**LR**: Left to Right

</td>
<td>

```mermaid
flowchart RL; 
    Start --> Middle --> End
```
**RL**: Right to Left

</td>
    </tr>
</table>

## Node Shape

```mermaid
flowchart LR; 
    1(Rounded) --> 2([Super rounded]) --> 3[[Bordered]] --> 4>Indented]
    5[/Slant right/] --> 6[\Slant left\] --> 7[/Squashed top\] --> 8[\Squashed bottom/]
    9[(Cylinder)] --> 10((Circle)) --> 11{Diamond} --> 12{{Hexagon}}
```
## Line Type

```mermaid
flowchart LR
    Basic --- 1[Basic with text] -- Text! --- End
    Dotted -.- 2[Dotted with text] -. Text! .- End
    Thick === 3[Thick with text] == Text! === End
```

## Arrow Type

```mermaid
flowchart LR
    Arrow --> 1[Arrow two way] <--> 2[Arrow with text] -- Text! --> End
    Circle --o 3[Circle two way] o--o 4[Circle with text] -- Text! --o End
    Cross --x 5[Cross two way] x--x 6[Cross with text] -- Text! --x End
```

## Link Types

```mermaid
flowchart LR
    1[Simple chain] --> Simple2 --> Simple3
    2[Split and combine] --> Split2 & Split3 --> Split4
    3[Multisplit] & Multisplit2 --> Multisplit3 & Multisplit4
```

## Link Length
```mermaid
flowchart LR
    Default --> Default2 --> Default3 --> Default4 --> Default5
    Long ---> Long2 ---> Long3
    Superlong -----> Superlong2

```
    
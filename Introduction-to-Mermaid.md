
# Main charts for Mermaid

::: mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
    D-->F;
    E-->F;
:::

### Here is the example code for the graph above:

        ::: mermaid
        graph TD;
            A-->B;
            A-->C;
            B-->D;
            C-->D;
            D-->F;
            E-->F;
        :::

## Sequence Diagram

::: mermaid
sequenceDiagram
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts!
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
:::

### Code for sequence diagram:

        ::: mermaid
        sequenceDiagram
            Alice->>John: Hello John, how are you?
            loop Healthcheck
                John->>John: Loop check
            end
            Note right of John: Note
            John-->>Alice: Great!
            John->>Bob: John to Bob
            Bob-->>John: Bob to John
        :::

## Gantt Chart

::: mermaid
gantt
title A Gantt Diagram
dateFormat YYYY-MM-DD
section Section 1
A task :a1, 2014-01-01, 30d
Another task :after a1 , 20d
another task : 24d
section Section 2
Task in sec :2014-01-12 , 20d
section Section 3
B task : a1, 2014-01-01, 30d
:::

### Code for gantt chart:

        ::: mermaid
        gantt
        title A Gantt Diagram
        dateFormat YYYY-MM-DD
        section Section 1
        A task :a1, 2014-01-01, 30d
        Another task :after a1 , 20d
        another task : 24d
        section Section 2
        Task in sec :2014-01-12 , 20d
        section Section 3
        B task : a1, 2014-01-01, 30d
        :::

## Class Diagram

:::mermaid
classDiagram
note "From Duck till Zebra"
Animal <|-- Duck
note for Duck "can fly\ncan swim\ncan dive\ncan help in debugging"
Animal <|-- Fish
Animal <|-- Zebra
Animal : +int age
Animal : +String gender
Animal: +isMammal()
Animal: +mate()
class Duck{
    +String beakColor
    +swim()
    +quack()
}
class Fish{
    -int sizeInFeet
    -canEat()
}
class Zebra{
    +bool is_wild
    +run()
}
:::
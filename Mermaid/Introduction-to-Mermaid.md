
# Main charts for Mermaid

## Graph

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
    Creature <|-- Superman
    Creature <|-- Vampire
    Creature <|-- Diavolo
    Creature: +int size
    Creature: +int weight
    Creature: +isBenign()
    Creature: +power()
    class Superman{
        +String currentName
        +fly()
        +heal()
    }
    class Vampire{
        -int age
        -canBite()
    }
    class Diavolo{
        +bool is_serving
        +heat()
    }
:::

### Here is the code to create the class diagram shown above

        :::mermaid
        requirementDiagram
        requirement development_req {
        id: 1
        text: requirements spec.
        risk: medium
        verifymethod: test
        }
        element test_suite {
        type: manual test
        }
        test_suite - verifies -> development_req
        :::

## Requirements Diagram

:::mermaid
requirementDiagram
    requirement development_req {
    id: 1
    text: requirements spec.
    risk: medium
    verifymethod: test
    }
    element test_suite {
    type: manual test
    }
    test_suite - verifies -> development_req
:::

### Code for Requirement Diagram shown above

        :::mermaid
        requirementDiagram
            requirement development_req {
            id: 1
            text: requirements spec.
            risk: medium
            verifymethod: test
            }
            element test_suite {
            type: manual test
            }
            test_suite - verifies -> development_req
        :::
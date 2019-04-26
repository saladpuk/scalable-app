# Scalable Application

Core concept is **Finding a bottleneck in a system**
![img](/images/bottleneck.PNG)

# Bottleneck
In software engineering, a bottleneck occurs when the capacity of an application or a computer system is severely limited by a single component, like the neck of a bottle slowing down the overall water flow. 

![img](/images/bottleneck_visualization.PNG)

# Bottleneck's Factors
1. OS
1. Software
1. Hardware
1. Environments
1. Database
1. Programming
1. Network
1. Bla bla bla ...

```
Bottlenecks ≠ one piece of shit
```

# Bottleneck
![img](/images/bottleneck_visualization.PNG)
```
Solving a single point does not mean that the problem is gone.
```


ideally making a single request (or no requests, as in a push protocol) rather than multiple roundtrips.

1. Progamming
    Algorithms and data structures (BigO)
    Language limitations (loop, recursive, structural & unstructured, string concatenation)
    Build & Compile level
    Strength reduction (sum of all integers from 1 to N)
    Bad code
    ```
    int i, sum = 0;
    for (i = 1; i <= N; ++i) {
    sum += i;
    }
    printf("sum: %d\n", sum);
    ```
    Good code
    ```
    int sum = N * (1 + N) / 2;
    printf("sum: %d\n", sum);
    ```

1. Poor database design
        Normalization
        Redundancy
        Bad Referential Integrity
        Not Taking Advantage of DB Engine Features { Views, Indexes, Stored procedures, Constraints, Triggers }
        No limitations on table or column name size
        Poor naming standards
        One table to hold all domain values
        Lack of testing
            Long & short running queries
            Write-write conflicts
            Large joins taking up memory

1. Software limitation


Design level
    Software design
    Network design
        network latency-bound
    Database design

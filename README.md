# Scalable Application

Core concept is **Finding bottlenecks in your system**
![img](/images/bottleneck.PNG)

# Bottleneck
In software engineering, a bottleneck occurs when the capacity of an application or a computer system is severely limited by a single component, like the neck of a bottle slowing down the overall water flow. 

![img](/images/bottleneck_visualization.PNG)

# Bottleneck's Factors
1. OS
1. Software
1. Hardware
1. Environments
1. Programming
1. Database
1. Network
1. Limitations
1. Bla bla bla ...

```
Bottlenecks ≠ one piece of shit
```

# Bottleneck
![img](/images/bottleneck_visualization.PNG)
```
Solving a single point does not mean that the problem is gone.
```

# Bottleneck's Factors - P2
1. Programming
1. Database
1. Limitations

# Progamming
* Algorithms and data structures
    * BigO
* Strategies
    * Query & NonQuery
    * Roundtrip
    * Connection pooling
* Language limitations
    * Loop
    * Recursive
    * Structural & Unstructured
    * String concatenation
* Build & Compile level

# Progamming (example)
The summation of all integers from 1 to N

Bad code
```
int i, sum = 0;
for (i = 1; i <= N; ++i)
{
    sum += i;
}
printf("sum: %d\n", sum);
```
Good code
```
int sum = N * (1 + N) / 2;
printf("sum: %d\n", sum);
```

# Database
*   Normalization
*   Redundancy
*   Bad Referential Integrity (1-1, 1-M, M-M)
*   Not Taking Advantage of DB Engine Features { Views, Indexes, Stored procedures, Constraints, Triggers }
*   No limitations on table or column name size
*   Poor naming standards
*   One table to hold all domain values
*   Lack of testing

# Database (example)
* Long & short running queries
* Write-write conflicts(Recursion tables)
* Large joins taking up memory

# Limitations
* Programming language (specialist like R, scalar)
* Database size
* Not support unstructured data
* Delete records

# Database techniques
* Caching
* Vertical & Horizontal Scaling
* Federation - Splitting into multiple DBs based on function
* Sharding - Splitting one dataset up across multiple hosts
* Moving some functionality to other types of DBs
???

# Database family
???

# Summary
* Finding bottlenecks in your system
* Bottlenecks ≠ one piece of shit
* Design level (Software, Database, Environments)
* Making a single request or no requests rather than multiple roundtrips
@title[Scalable Application]

## Scalable Application

---

@title[Goal]

### Scalable Application Goal

@size[0.75em](@fa[quote-left] Core concept is **Finding bottlenecks in your system** @fa[quote-right])
![img](/images/bottleneck.PNG)

---

@title[What's buttleneck]

## What's buttleneck
@size[0.75em](In software engineering, a bottleneck occurs when the capacity of an application or a computer system is severely limited by a single component, like the neck of a bottle slowing down the overall water flow.)

![img](/images/bottleneck_visualization.PNG)

---

@title[Bottleneck's factors]
### Bottleneck's factors
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

---

@title[Bottleneck summary]

## Bottleneck summary
![img](/images/bottleneck_visualization.PNG)
```
Solving a single point does not mean that the problem is gone.
```

---

@title[Bottleneck's factors - Part 2]

## Bottleneck's factors 2
1. Programming
1. Database
1. Limitations

---

@title[Progamming]

### Progamming
* Algorithms and data structures (BigO)
* Strategies
    * Query & NonQuery (Pagging, LIMIT)
    * Roundtrip
    * Connection pooling
* Language limitations
    * Loop & Recursive
    * Structural & Unstructured
    * String concatenation
* Build & Compile level

---

@title[Progamming (example 1)]

### Progamming (example)
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

---

@title[Database 1]

### Database 1
* Normalization
* Redundancy
* Bad Referential Integrity (1-1, 1-M, M-M)
* Not Taking Advantage of DB Engine Features { Views, Indexes, Stored procedures, Constraints, Triggers }
* No limitations on table or column name size
* One table to hold all domain values
* Lack of testing

---

@title[Database 2]

### Database 2
* Poor design
    * Fixed length of data
    * Not use datatypes based on the nature of data
    * Naming standards

---

@title[Database (example)]

## Database (example)
* Long & short running queries
* Write-write conflicts(Recursion tables)
* Large joins taking up memory
```
the number of queries you can handle at a time
```

---

@title[Limitations]

## Limitations
* Programming language (specialist like R, scalar)
* Database size
* Not support unstructured data
* Delete records (Hole & Indexes)

---

@title[Database techniques]

## Database techniques
* Design guideline & Best practices
    * [InnoDB Tables](https://dev.mysql.com/doc/refman/8.0/en/innodb-best-practices.html)
* Caching
* Hot & Cold data
* Vertical & Horizontal Scaling
* Federation - Splitting into multiple DBs based on function
* Sharding - Splitting one dataset up across multiple hosts
* Moving some functionality to other types of DBs

---

@title[Database types]

## Database types
* Relational database
* Non-Relational database (NoSQL)

---

@title[Relational database]

## Relational database
is a digital database based on the relational model of data
![img](/images/relational_db.png)


**Disadvantages**
* Cannot store complex or very large images

---

@title[Non-Relational database (NoSQL)]

### Non-Relational database (NoSQL)
Originally referring to **non SQL** or **non relational**

* **Advantages**
> Large volumes of structured, semi-structured, and unstructured data

* **Disadvantages**
> Less support since NoSQL databases are usually open-source

---

@title[NoSQL family]

## NoSQL family
* Graph ([neo4J](https://console.neo4j.org), OrientDB, Titan)
* Key-Value store ([Redis](https://try.redis.io), Amazon DynamoDB)
* Document database ([MongoDB](https://www.mplay.run/mongodb-online-terminal), Couchbase)
* Column store (Apache HBase, Cassandra)

---

@title[Summary]

## Summary
* Finding bottlenecks in your system
* Bottlenecks ≠ one piece of shit
* Design level (Software, Database, Environments)
* Making a single request or no requests rather than multiple roundtrips
* The number of queries you can handle at a time

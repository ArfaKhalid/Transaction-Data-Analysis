# Transaction Data Management 

This repository reflects my exploration of PostgreSQL's transaction management capabilities, focusing on a table called `bank_accounts`. Join me as I walk through the creation of the table, showcase atomic transactions, demonstrate rollback scenarios, and delve into various transaction isolation levels.

## Table of Contents

1. [Table Creation and Initial Data Insertion](#table-creation)
2. [Atomic Transactions](#atomic-transactions)
3. [Rolling Back Transactions](#rollback-transactions)
4. [Savepoints](#savepoints)
5. [Transaction Isolation Levels](#transaction-isolation-levels)
    - [READ COMMITTED](#read-committed)
    - [REPEATABLE READ](#repeatable-read)
    - [SERIALIZABLE](#serializable)
6. [Conclusion](#conclusion)

---

## 1. Table Creation and Initial Data Insertion <a name="table-creation"></a>

I start by creating a new table called `bank_accounts`, which will store essential information about various bank accounts. Initial data insertion showcases examples with individuals like Charlie, Dora, and Jack.

## 2. Atomic Transactions <a name="atomic-transactions"></a>

I explore the concept of atomic transactions, ensuring a sequence of steps is executed atomically. Examples include debiting and crediting amounts to different accounts within a single transaction block.

## 3. Rolling Back Transactions <a name="rollback-transactions"></a>

Learn how to roll back transactions using the `ROLLBACK` command. I provide scenarios where transactions are rolled back, preserving the integrity of the data.

## 4. Savepoints <a name="savepoints"></a>

Savepoints offer flexibility within a transaction. I demonstrate their use in rolling back to specific points, allowing for more nuanced management of changes.

## 5. Transaction Isolation Levels <a name="transaction-isolation-levels"></a>

Dive into different transaction isolation levels provided by PostgreSQL and understand their impact on concurrent transactions.

### READ COMMITTED <a name="read-committed"></a>

Explore how the `READ COMMITTED` isolation level allows changes to be visible only after a transaction is committed.

### REPEATABLE READ <a name="repeatable-read"></a>

Discover the `REPEATABLE READ` isolation level, preventing changes in the same transaction from affecting subsequent reads.

### SERIALIZABLE <a name="serializable"></a>

Examine the `SERIALIZABLE` isolation level, which prevents concurrent transactions from making changes to the same data simultaneously.

## 6. Conclusion <a name="conclusion"></a>

This project provides a hands-on experience with SQL commands and transaction management, offering a solid foundation for working with financial data in a relational database.



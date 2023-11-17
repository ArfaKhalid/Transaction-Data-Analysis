# Transaction-Data-Analysis
## Bank Transaction Management

Welcome to the Bank Transaction Management project! This repository guides you through the process of creating a new table called `bank_accounts` and demonstrates various transaction management scenarios using PostgreSQL. Whether you're dealing with simple inserts, updates, rollbacks, or exploring different transaction isolation levels, this project provides hands-on examples and explanations.

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

We start by creating a new table called `bank_accounts` to store information about bank accounts. The table includes columns for `id`, `name`, and `balance`. Initial data insertion is demonstrated with examples of inserting accounts for individuals like Charlie, Dora, and Jack.

## 2. Atomic Transactions <a name="atomic-transactions"></a>

This section introduces the concept of atomic transactions, where a sequence of steps needs to be executed atomically. Examples include debiting and crediting amounts to different accounts within a single transaction block, ensuring that the changes are applied together.

## 3. Rolling Back Transactions <a name="rollback-transactions"></a>

Explore how to roll back transactions using the `ROLLBACK` command. Examples demonstrate scenarios where transactions are rolled back, preserving the integrity of the data.

## 4. Savepoints <a name="savepoints"></a>

Savepoints allow you to create intermediate points within a transaction. This section illustrates the use of savepoints to roll back to specific points in the transaction, maintaining flexibility in managing changes.

## 5. Transaction Isolation Levels <a name="transaction-isolation-levels"></a>

Dive into different transaction isolation levels provided by PostgreSQL and understand their impact on concurrent transactions. Explore scenarios under "READ COMMITTED," "REPEATABLE READ," and "SERIALIZABLE" isolation levels.

### READ COMMITTED <a name="read-committed"></a>

Demonstrates how the `READ COMMITTED` isolation level allows changes to be visible only after a transaction is committed.

### REPEATABLE READ <a name="repeatable-read"></a>

Explores the `REPEATABLE READ` isolation level, preventing changes in the same transaction from affecting subsequent reads.

### SERIALIZABLE <a name="serializable"></a>

Examines the `SERIALIZABLE` isolation level, which prevents concurrent transactions from making changes to the same data simultaneously.

## 6. Conclusion <a name="conclusion"></a>

This project provides hands-on experience with SQL commands and transaction management, offering a solid foundation for working with financial data in a relational database.




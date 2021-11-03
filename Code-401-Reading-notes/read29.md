# [Save data in a local database using Room](https://developer.android.com/training/data-storage/room)

The most common use case is to cache relevant pieces of data so that when the device cannot access the network, the user can still browse that content while they are offline.

Room provides the following benefits:
 - Compile-time verification of SQL queries.
 - Convenience annotations that minimize repetitive and error-prone boilerplate code.
 - Streamlined database migration paths.

## Primary components

- The database class that holds the database and serves as the main access point for the underlying connection to your app's persisted data.
- Data entities that represent tables in your app's database.
- Data access objects (DAOs) that provide methods that your app can use to query, update, insert, and delete data in the database.



# [Defining data using Room entities](https://developer.android.com/training/data-storage/room/defining-data)

When you use the Room persistence library to store your app's data, you define entities to represent the objects that you want to store. Each entity corresponds to a table in the associated Room database, and each instance of an entity represents a row of data in the corresponding table.

## Anatomy of an entity

You define each Room entity as a class that is annotated with `@Entity`. A Room entity includes fields for each column in the corresponding table in the database, including one or more columns that comprise the primary key.

## Define a primary key

Each Room entity must define a primary key that uniquely identifies each row in the corresponding database table.



## Ignore fields
By default, Room creates a column for each field that's defined in the entity. If an entity has fields that you don't want to persist, you can annotate them using `@Ignore`.

# [Define relationships between objects](https://developer.android.com/training/data-storage/room/relationships)

In Room, there are two ways to define and query a relationship between entities: you can model the relationship using either an intermediate data class with embedded objects, or a relational query method with a multimap return type.


# [Accessing data using Room DAOs](https://developer.android.com/training/data-storage/room/accessing-data#java)

When you use the Room persistence library to store your app's data, you interact with the stored data by defining data access objects, or DAOs. Each DAO includes methods that offer abstract access to your app's database. At compile time, Room automatically generates implementations of the DAOs that you define.
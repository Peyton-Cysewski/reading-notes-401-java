# Room

## Saving Data Locally
There are 3 major components in Room:
- Database: Contains the database holder and serves as the main access point for the underlying connection to your app's persisted, relational data.
- Entity: Represents a table within the database.
- DAO: Contains the methods used for accessing the database.

## Entities
- When using the Room persistence library, you define sets of related fields as entities. For each entity, a table is created within the associated Database object to hold the items. You must reference the entity class through the entities array in the Database class.
- Each entity must define at least 1 field as a primary key. Even when there is only 1 field, you still need to annotate the field with the `@PrimaryKey` annotation. Also, if you want Room to assign automatic IDs to entities, you can set the `@PrimaryKey`'s autoGenerate property. If the entity has a composite primary key, you can use the primaryKeys property of the `@Entity` annotation.
- You can use the `@Embedded` annotation to represent an object that you'd like to decompose into its subfields within a table. This is what allows an entity to directly reference another.

## Accessing Data
The DAO as denoted by `@Dao` is what creates the query statements for the internal database. It can auto-generate queries, but you can also define custom ones for specific use cases.


[Table of Contents](../README.md)


### External Links
- [Overview: Saving data with Room](https://developer.android.com/training/data-storage/room)
- [Defining entities in Room](https://developer.android.com/training/data-storage/room/defining-data)
- [Related entities in Room](https://developer.android.com/training/data-storage/room/relationships)
- [Accessing data with Room](https://developer.android.com/training/data-storage/room/accessing-data#java)
# JFSD-Inheritance-mapping
Inheritance Mapping in Hibernate
Inheritance mapping is a powerful feature in Hibernate that allows you to map Java class hierarchies to database tables. This technique is essential for modeling real-world entities that share common properties while also having unique attributes. Inheritance mapping can simplify your database design and make your application more flexible and easier to maintain.

Types of Inheritance Mapping Strategies
Hibernate supports several strategies for inheritance mapping, each with its own advantages and trade-offs:

Table Per Class Hierarchy (Single Table Strategy):

Description: All classes in the hierarchy are mapped to a single database table.
Pros: Simple and efficient with a single table query.
Cons: Can result in sparse tables with many nullable columns.
Table Per Subclass (Joined Strategy):

Description: Each class in the hierarchy is mapped to its own table, and tables are joined together using primary and foreign keys.
Pros: Normalized database structure, avoids null columns.
Cons: More complex queries and joins.
Table Per Concrete Class (Table Per Class Strategy):

Description: Each concrete class in the hierarchy is mapped to its own table.
Pros: Simple table structure, no joins required for concrete classes.
Cons: Data redundancy, difficulty querying across the hierarchy.

### Chapter Two: Data Models and Query Languages
1. Different Data Models
    1. Relational Model
        1. Data is organized into "relations"
        2. Each "relation" is an unordered collection of "tuples" (rows in SQL)
        3. A "tuple" is an immutable data structure containing an ordered
           seqeuence of elements
        4. Requires a non-flexible schema
    2. Document Model
        1. Typically no enforced schema structure
        2. Not good for displaying many to many relationships
        3. Great at storing self-contained data, such as a resume
    3. Graph Model
        1. Typically no enforced schema structure
        2. Excels in many to many relationships
2. NoSQL: "Not only SQL"
3. Data models can be emulated by another data model. Ex: A graph model could
   be represented by a relational model, though it will likely be much more
   difficult and/or awkward
4. Query Languages
    1. Every data model has its own query language. Given the breadth of this
       topic, I will add query language examples in the chapters that focus on
       them


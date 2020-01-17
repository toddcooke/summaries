# summaries

ACID
- Atomic - The transaction completely succeeds or falis
- Consistent - Data will be valid before and after a transaction
- Isolated - Transactions can happen concurrently
- Durable - The results of a transaction are saved to disk

Eventual Consistency - Reads after writes may not reflect latest writes

REST - Representational State Transfer
1. Client-Server - Client and server can change independently: they are decoupled
1. Stateless - Server does not retain state of client
1. Cacheable - Some responses may be cached by the server
    - GET and HEAD
    - 200, 203, 204, 206, 300, 301, 404, 405, 410, 414, and 501
    - No cache preventing headers, like Cache-Control
1. Uniform Interface
    - Resource identification in requests - eg Content-Type
    - Resource manipulation through representations
    - Self-descriptive messages
    - Hypermedia as the engine of application state (HATEOAS)
1. Layered System - clients don't know whether they are connected directly to end server, or are going through an intermediary
1. (Optional) Code on demand - servers can transfer executable code

Software Architecture Patterns
- Event sourcing - Append only data store records all events that occur
- Strangler pattern - Facade allows old system to be slowly replaced

Software Design Patterns
- Factory Method - A method creates a new object without directly instantiating 

SQL
- Inner join - All rows from tables A and B where a condition is met
- Left outer join - Same as inner join plus all rows from the left side of the JOIN operator
- Right outer join - Same as inner join plus all rows from the right side of the JOIN operator
- Full outer join - All rows from both tables
- WHERE - can't have aggregate functions. Selects input rows before groups and aggregates are computed
- HAVING - always has aggregate functions. Selects group rows after groups and aggregates are computed

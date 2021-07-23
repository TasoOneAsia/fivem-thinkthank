---------------
Component: 'Core';
Feature: 'Database';
---------------

## Database Functionality

The database is included within the Core resource for several reasons.

1. A persistent store is inherently a `core` feature of any extendable framework
2. As the `Core` resource on the server side is planned to be primarily in the V8 ScRT, aside from bridging.
   Database heavy functionality induced by other modules such as the *Player Manager* would be able to
   efficiently call and handle queries without incurring penalties of a standalone database resource (serialization,
   event overhead etc)
   
*I am thinking PostGres is a nice mix between some NoSQL paradigms and relational, while keeping the familiar syntax
and functionality of the most common drivers in use at the moment* 
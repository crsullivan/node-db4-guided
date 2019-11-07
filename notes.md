# Data Modeling Notes

## Requirements

A client has hired you to build an API for managing `zoos` and the `animals` kept at each `zoo`. The API will be use for `zoos` in the _United States of America_, no need to worry about addresses in other countries.

For the `zoos` the client wants to record:

- name.
- address.

For the `animals` the client wants to record:

- name.
- species.
- list of all the zoos where they have resided.

Determine the database tables necessary to track this information.
Label any relationships between table.

## A Good Data Model

- captures ALL the data the system needs
- captures ONLY the data the system needs
- reflect reality (from the point of view of the system)
- is flexible, can evolve with the system
- guarantees data integrity without sacrificing too much performance
- is driven by the way we access data

## Components

- entities (nouns: zoo, animal, species), like a resource ---> tables
- properties ---> columns, fields
- relationships ---> foreign keys

## Workflow 

- identify entities ("real", and "transactional" (luis lingo))
- identify properties
- identify relationships

## Relationships
- one to one
- one to many (most common) _there are many animals in one species_
- many to many (smoke and mirrors)


## Mantras

- every table must have a primary key
- work on two or three entities at a time
- one to many relationships are formed using a foreign key
- the foreign key column must be the same type as the primary key it references
- many to many relationships are modeled using a third table
- this third table could include columns other than just foreign keys
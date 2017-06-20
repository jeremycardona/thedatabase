# Relational Modeling

A model describes data or information.

### relations
a relation is a way of representing a two dimensional table
### attributes
attributes are the column names of a relation

Lets say we want to define a relation we attributes:

R(a1, a2, ..., an)
where R is the *name of the relation*
where a1, a2,..,an are the *names of the attributes*

for example lets say we want to represent a table that contains information of beers:
Beer(id, name, brewery, adv, style)


# Tuples
a tuple is a single component for each attribute of a relation
example with beers:
(1, 'Medalla', 'Brewery of Puerto Rico', 4.0, 'light')


# Keys
we want to have an attribute or attributes such that they for a key, which is a way of identifying a tuple
lets say for example we have a relation with a lot of values, we want to have a way of getting a single tuple:
for example:
Beer(*id*, name, brewery, adv, style)
where id is an identifier or unique key for beers 

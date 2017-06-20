# Relational design

We could design a relational schema (database tables) of many ways. Having a good design is important especially for eliminating redundancy. 

### functional dependency
functional dependency is a way of having a set of attributes {A1, A2, ..., An} determine all other attributes {B1, B2, ... Bn}.
if {A1, A2, ..., An} functionally determines all other attributes it is said to be a key.
lets have for example the tuple: Beer(id, name, brewery, adv, style)
id functionally determines name, brewery, adv, style

### design of schemas
Bad design can lead to anomalies and redundancies so, often is a good idea to decompose the relation to avoid this.
anomalies can be redundancies where information is repeated unnesesarily. Update anomalies can be another where we change information in one tuple but leave it unchanged in another. Deletion anomalies is where a set of values become empty and we may lose other information as a side effect.

a way to deal with this is to decompose relations. Decomposition of a relation involves splitting the attributes to make the schemas of
two new relations.

### normal forms

*Boyce codd normal form*
A relation is in BCNF if and only if: whenever there is a nontrivial FD
A1, A2, .., An --> B1, B2,..., Bm for the Relation, it is the case that {A1, A2, .., An} is
a superkey for R.
That is, the left side of every nontrivial FD must be a superkey. 

*Third normal form*
3NF condition can be stated as “for each nontrivial FD, either the left side is a
superkey, or the right side consists of attributes that are a member of some key only.”


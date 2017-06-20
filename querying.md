# Relational Querying

We want to have a way to access our data an do operation with it
### operations
lets say we have two relations R and S 
_union_ : the union of R and S is the set of elements that are in R or S or both.
_intersection_: the intersection of R and S is the set of elements that are in both
_difference_: the difference of R and S is the set of element that are in R but not in S

### projection
its a way of creating a new relation that have some columns of a relation
we have the relation Beer(id, name, brewery, adv, style)
the projection of name from Beer, would result in a new relation Beer(name)

### selection
a selection to an relation would produce a subset of the relation tuples
we can make selections in the form of 
select{condition} from R which is going to return all tuples that are true to the condition
for example:
select{adv > 5.0} from Beer would return all beers that have adv greater than 5.0

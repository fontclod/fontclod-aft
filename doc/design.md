not really to complicated -- needs to be able
to do the following:

1. store users and authenticate them

2. store fonts

3. back up


# users

simplest thing would probably be to use redis.
it's relatively quick and there wont be a lot
to store there at first. later it can also be
used as a cache if that becomes necessary

## "schema"

node_id - hex prefix like "6e" to be used in ids

user_counter - incremented number

user:6e1001 - hash

    name "Edward Newgate"
    email ""
    passwd "hash" 
    plan 1

user_plans - sorted set (weight is plan id)

there may also be some "index records" for
a few things


# font files

simplest way to do this would probably be mongo.
we can store clodifle in it basically unchanged,
and make changes to just parts of the tree,
or add indexes to fields we think is necessary


# back up

most likely this can use an s3-compatible storage,
and also possibly something like glacier for
long-term back ups

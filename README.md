# MySQL Tuning Primer

This fork is taken from:
- https://launchpad.net/mysql-tuning-primer/trunk

This fork was made on revision:
- matt.montgomery@sun.com-20110902034720-07nbdf7z3kudqtdv

# Usage

Find an instance that is able to connect to the RDS you wish to profile. Go to that instance's stack's
dashboard and run the command 'Execute Recipes'. Configure the recipe
`ies-mysql-tuning-primer::default` to run on the instance you've investigated. This will deploy the
primer script under `/usr/local/bin/ies-mysql-tuning-primer.sh`.

SSH onto the instance, create `~/.my.cnf'...

```
[client]
user = 
password = 
hostname = 
```

... end fill out the blanks.

Finally, execute the script:
```
ies-mysql-tuning-primer.sh
```

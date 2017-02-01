# Inventory
Platform for managing custom inventories

## Getting The Project

### Fork
Fork your own copy of the [Inventory](https://github.com/harold20/Inventory/fork) repository to your account

### Clone
Get a copy of your recently cloned version of console in your machine.
```
$ git clone git@github.com:[your-git-user-here]/Inventory.git
```


### Configure a remote fork
```
$ git remote add upstream https://github.com/harold20/Inventory.git
```

### Sync your fork
```
$ git fetch upstream
$ git merge upstream/master
```

### Install dependencies
```
$ composer install
```


Provide the MySQL user credentials created in the previous step.


### Update database schema
```
$ bin/console doctrine:migrations:migrate
```

### Sync database schema
```
$ bin/console doctrine:migrations:diff
```

### Generate super-admin user
```
$ bin/console fos:user:create admin --super-admin
```

# doctrine-sql-logger
Debug Doctrine 2 real SQL queries with parameters

## Installation

composer require cmyker/doctrine-sql-logger:dev-master

## Usage example

```php
$connection = $this->getEntityManager()->getConnection(); 
$logger = new \Cmyker\DoctrineSqlLogger\Logger($connection);
$connection->getConfiguration()->setSQLLogger($logger);
//some query here
echo $logger->lastQuery; //or see the output
```

TODO more details

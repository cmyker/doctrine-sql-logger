# doctrine-sql-logger
Debug Doctrine 2 real SQL queries with parameters

Installation

composer require cmyker/doctrine-sql-logger:dev-master

Usage example

$connection = $this->getEntityManager()->getConnection();
$connection->getConfiguration()->setSQLLogger(new \Cmyker\DoctrineSqlLogger\Logger($connection));

TODO more details

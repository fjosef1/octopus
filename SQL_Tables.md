<h1>Creating the Database and Tables</h1>

Create a database called octopus:
```
CREATE DATABASE octopus;
```

Now login and create the energy_consumption table 

```
CREATE TABLE `energy_consumption` (
  `id` int NOT NULL AUTO_INCREMENT,
  `consumption` decimal(12,3) NOT NULL,
  `interval_start` datetime NOT NULL,
  `interval_end` datetime NOT NULL,
  PRIMARY KEY (`id`)
);
```

Now create the unit_rates table so we can store the market prices 
```
CREATE TABLE `unit_rates` (
  `id` int NOT NULL AUTO_INCREMENT,
  `value_exc_vat` decimal(10,2) NOT NULL,
  `value_inc_vat` decimal(10,3) NOT NULL,
  `valid_from` datetime DEFAULT NULL,
  `valid_to` datetime DEFAULT NULL,
  PRIMARY KEY (`id`)
);
```

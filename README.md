# MYSQL   

**CREATE SCHEMA**  
~~~
CREATE SCHEMA `schema_name` DEFAULT CHARACTER SET utf8 ;
~~~

**CREATE TABLE**
~~~
CREATE TABLE board`.`Board` (  
  `idx` INT NOT NULL AUTO_INCREMENT,  
  `name` VARCHAR(45) NOT NULL,  
  `password` VARCHAR(45) NOT NULL,  
  `subject` VARCHAR(500) NOT NULL,  
  `content` VARCHAR(5000) NULL,  
  `readCount` INT NULL DEFAULT 0,  
  `wdate` DATETIME NULL,  
  `enterprise` VARCHAR(45) NULL,  
  `cpuname` VARCHAR(45) NULL,  
  `socket` VARCHAR(45) NULL,  
  `speed` VARCHAR(45) NULL,  
  `core` INT NULL,  
  `thread` INT NULL,  
  `graphis` VARCHAR(45) NULL,  
  `filePath` VARCHAR(45) NULL,  
  `fileName1` VARCHAR(45) NULL,  
  `fileName2` VARCHAR(45) NULL,  
  PRIMARY KEY (`idx`));  
  ~~~
***ALTER TABLE***
~~~  
ALTER TABLE `board`.`Board` 
ADD COLUMN `addFile` VARCHAR(45) NULL AFTER `fileName2`;
~~~
~~~
ALTER TABLE `board`.`Board` 
DROP COLUMN `addFile`;
~~~

***INSERT***
~~~
INSERT INTO `board`.`Board` (`name`, `password`) VALUES ('test', '1234');
~~~

***UPDATE***
~~~
UPDATE `board`.`Board` SET `content` = 'test' WHERE (`idx` = '1');
~~~

# MYSQL   
//-------------------------  
**CREATE SCHEMA**  
CREATE SCHEMA `schema_name` DEFAULT CHARACTER SET utf8 ; <-default charcter utf-8   

**CREATE TABLE**
CREATE TABLE board`.`Board` ( </>
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
  

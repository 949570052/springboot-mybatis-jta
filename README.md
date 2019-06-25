# springboot-mybatis-jta
整合springboot,mybatis,jta   实现分布式事务 很经典 atomikos-jta 


sql 

自己建个test库和test2库 两个库的表结构都是一样的直接把下面的语句丢进去，不多说

SET FOREIGN_KEY_CHECKS=0;

-- ----------------------------
-- Table structure for test
-- ----------------------------
DROP TABLE IF EXISTS `test`;
CREATE TABLE `test` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `name` varchar(255) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=9 DEFAULT CHARSET=utf8;

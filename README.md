# yuchenerp    newdemo


sql：

/*
Navicat MySQL Data Transfer

Source Server         : yuchen
Source Server Version : 80016
Source Host           : localhost:3306
Source Database       : yuchengerp

Target Server Type    : MYSQL
Target Server Version : 80016
File Encoding         : 65001

Date: 2020-11-27 15:04:49
*/

SET FOREIGN_KEY_CHECKS=0;

-- ----------------------------
-- Table structure for user
-- ----------------------------
DROP TABLE IF EXISTS `user`;
CREATE TABLE `user` (
  `id` int(11) NOT NULL,
  `username` varchar(255) NOT NULL COMMENT '用户名',
  `password` varchar(255) NOT NULL COMMENT '密码',
  `tel` varchar(255) NOT NULL COMMENT '手机号码',
  `age` int(255) DEFAULT NULL COMMENT '年龄',
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;

-- ----------------------------
-- Records of user
-- ----------------------------
INSERT INTO `user` VALUES ('1', 'zhangsan', 'zhangsan666', '18087474922', '22');
INSERT INTO `user` VALUES ('2', 'lisi', '12345678', '19938489929', '33');
INSERT INTO `user` VALUES ('3', 'wangwu', 'qweradc', '18087202644', '35');

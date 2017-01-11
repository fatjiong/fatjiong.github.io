---
layout: post
title:  "【Queue】新手安装并使用Beanstalked"
categories: 技术
tags:  Queue Beanstalked
author: 胖纸囧
---

* content
{:toc}

因为公司项目准备要重构，根据当前业务的复杂度，为了降低系统业务耦合程度，需要在项目中引入消息队列机制。

## 资料

在使用之前先来点资料普及下什么是消息队列，还有消息队列有什么用：

- [消息队列](http://baike.baidu.com/link?url=JOv29wGjBmYc32hlY9v8yAfcs925V0mA5n-ZBVUcNu_JMSr1Xkd0I4t6Uby0us5y_JFAU4a71QWUf16QyOv4SzIidc1YZ2G7ho5GO0u-42WnCMS--rflOrw4nZlS4zUX)
- [消息队列有什么用？](https://segmentfault.com/q/1010000005780973)
- [PHP实现队列及队列原理](http://www.phpddt.com/php/queue.html)
- [大型网站架构之分布式消息队列](http://blog.csdn.net/shaobingj126/article/details/50585035)

## 候选

在当前的技术前景下，有以下几种队列选择：

- [JMS](http://baike.baidu.com/link?url=U2WYoeoyDZ1UdtsINkRQObR9rrDRviRDI9gfMpZ1QWl8mhAz5b20FfsYYyFEqF1Y2we9KJ4VMCso4uYziIVn_K)
- [RabbitMQ](http://www.rabbitmq.com)
- [ZeroMQ](http://www.zeromq.org)
- [Kafka](http://kafka.apache.org)
- [beanstakd](http://baike.baidu.com/link?url=CwcW0w5-TLS1DFIhqfMr-TFV_Z5vKxHQALdLxVMoX9rG4qLowucBokmVUFkuvtIECR59cR-iVBHTk_yoRm6s8ncSxh_-WHkdPb9uEubuciG)

## 核心

![](media/14836920498907/14841019778243.jpg)


Beanstalkd设计里面的核心概念：
* job
* tube
* producer
* consumer

## 安装


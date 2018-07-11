# PHP interview best practices in China


## 基础篇
* 了解大部分数组处理函数
* 字符串处理函数（区别 mb_ 系列函数）
* & 引用，结合案例分析
* == 与 === 区别
* isset 与 empty 区别
* 全部魔术函数理解
* static、$this、self 区别
* private、protected、public、final 区别
* OOP 思想
* 抽象类、接口 分别使用场景
* Trait 是什么东西
* echo、print、print_r 区别
* __construct 与 __destruct 区别
* static 作用（区分类与函数内）
* __toString() 作用
* 单引号’ 与双引号 “ 区别
* 常见 HTTP 状态码，分别代表什么含义
* 301 什么意思 404 呢

## 进阶篇
* Autoload、Composer 原理
* Session 共享、存活时间
* 异常处理
* 如何 foreach 迭代对象
* 如何数组化操作对象 $obj[key]
* 如何函数化对象 $obj(123);
* yield 是什么，说个使用场景
* PSR 是什么，PSR-1, 2, 4, 7
* 如何获取客户端 IP 和 服务端 IP 地址
* 如何开启 PHP 异常提示
* 如何返回一个301重定向
* 如何获取扩展安装路径
* 字符串、数字比较大小的原理，注意 0 开头的8进制、0x 开头16进制
* BOM 头是什么，怎么除去
* 什么是 MVC 
* 依赖注入实现原理
* 如何异步执行命令
* 模板引擎是什么，解决什么问题、实现原理（Smarty、Twig、Blade）
* 如何实现链式操作 $obj->w()->m()->d();
* Xhprof 、Xdebug 性能排除工具使用

## 实践篇
* 给定二维数组，根据某个字段排序
* 如何判断上传文件类型，如：仅允许 jpg 上传
* 不使用临时变量交换两个变量的值 $a=1; $b=2;  =>  $a=2; $b=1
* strtoupper 在转换中文时存在乱码，你如何解决？ echo strtoupper(‘ab你好c’);
* Websocket、Long-Polling、Server-Sent Events(SSE) 区别
* “Headers already sent” 错误是什么意思，如何避免

## 算法篇
* 快速排序（手写）
* 冒泡排序（手写）
* 二分查找（了解）
* 查找算法 KMP（了解）
* 深度、广度优先搜索（了解）

## 数据结构篇（了解）
* 堆、栈特性
* 队列
* 哈希表
* 链表

## 对比篇
* Cookie 与 Session 区别
* GET 与 POST 区别
* include 与 require 区别
* include_once 与 require_once 区别
* Memcached 与 Redis 区别
* MySQL 各个存储引擎、及区别（一定会问  MyISAM 与 Innodb 区别）
* HTTP 与 HTTPS 区别
* Apache 与 Nginx 区别
* define() 与 const 区别
* traits 与 interfaces 区别 及 traits 解决了什么痛点？
* Git 与 SVN 区别

## 数据库篇
* MySQL
    * CRUD
    * JOIN、LEFT JOIN 、RIGHT JOIN、INNER JOIN
    * UNION
    * GROUP BY + COUNT +WHERE 组合案例
    * 常用 MySQL 函数，如：now、md5、concat、uuid 等
    * 1:1、1:n、n:n 各自适用场景
    * 数据库优化手段
        * 索引、联合索引（命中条件）
        * 分库分表
        * 分区
        * 会使用 explain 分析 SQL 问题，了解各参数含义
        * Slow Log（有什么用，什么时候需要）
* MSSQL(了解)
    * 查询最新5条数据
* NOSQL
    * Redis、Memcached、MongoDB
    * 对比、适用场景
    * 你之前为了解决什么问题使用的什么，为什么选它？

## 服务器篇
* 查看 CPU、内存、时间、系统版本等信息
* find 、grep 查找文件
* awk 处理文本
* 查看命令所在目录
* 自己编译过 PHP 吗？如何打开 readline 功能
* 如何查看 PHP 进程的内存、CPU 占用
* 如何给 PHP 增加一个扩展
* 修改 PHP Session 存储位置、修改 INI 配置参数
* 负载均衡有哪几种，挑一种你熟悉的说明其原理
* 数据库主从复制 M-S 是怎么同步的？是推还是拉？会不会不同步？怎么办
* 如何保障数据的可用性，即使被删库了也能恢复到分钟级别。你会怎么做。
* 数据库连接过多，超过最大值，如何优化架构。从哪些方便处理？
* 502 大概什么什么原因？ 如何排查  504呢？

## 架构篇
* 偏运维（了解）：
    * 负载均衡（Nginx、HAProxy、DNS）
    * 主从复制（MySQL、Redis）
    * 数据冗余、备份（MySQL增量、全量 原理）
    * 监控检查（分存活、服务可用两个维度）
    * MySQL、Redis、Memcached Proxy 、Cluster 目的、原理
    * 分片
    * 高可用集群
    * RAID
    * 源代码编译、内存调优
* 缓存
    * 工作中遇到哪里需要缓存，分别简述为什么
* 搜索解决方案
* 性能调优
* 各维度监控方案
* 日志收集集中处理方案
* 国际化
* 数据库设计
* 静态化方案

## 框架篇
* ThinkPHP（TP）、CodeIgniter（CI）、Zend（非 OOP 系列）
* Yaf、Phalcon（C 扩展系）
* Yii、Laravel、Symfony（纯 OOP 系列）
* Swoole、Workerman （网络编程框架）
* 对比框架区别

## 设计模式
* 单例模式（重点）
* 工厂模式（重点）
* 观察者模式（重点）
* 装饰器模式
* 依赖注入（重点）
* 代理模式
* 组合模式

## 安全篇
* SQL 注入
* XSS 与 CXRF
* 输入过滤
* Cookie 安全
* 禁用 mysql_ 系函数
* 数据库存储用户密码时，应该是怎么做才安全
* 验证码 Session 问题
* 安全的 SESSION ID （让即使拦截后，也无法模拟使用）
* 目录权限安全
* 包含本地与远程文件
* 文件上传脚本
* eval 函数执行脚本
* disable_functions 关闭高位函数
* FPM 独立用户与组，目录特定权限
* 了解 hash 与 encrypt 区别

## 高阶篇
* PHP 数组底层实现 （HashTable + Linked list）
* Copy on write 原理，何时 GC
* PHP 进程模型，进程通讯方式，进程线程区别
* yield 核心原理是什么
* PDO prepare 原理
* PHP 7 与 PHP 5 有什么区别
* Swoole 适用场景，协程实现方式

## 前端篇
* 原生获取 DOM 节点，属性
* 盒子模型
* CSS 文件、<style> 标签、行内 style 属性优先级
* HTML 与 JS 运行顺序（页面 JS 从上到下）
* JS 数组操作
* 类型判断
* this 作用域
* .map() 与 this 具体使用场景分析
* Cookie 读写
* JQuery 操作
* Ajax 请求（同步、异步区别）随机数禁止缓存
* Bootstrap 有什么好处
* 跨域请求 N 种解决方案
* 新技术（了解）
    * ES6
    * 模块化
    * 打包
    * 构建工具
    * vue、react、webpack、
    * 前端 mvc 
* 优化
    * 浏览器单域名并发数限制
    * 静态资源缓存 304 （If-Modified-Since 以及 Etag 原理）
    * 多个小图标合并使用 position 定位技术 减少请求
    * 静态资源合为单次请求 并压缩
    * CDN
    * 静态资源延迟加载技术、预加载技术
    * keep-alive
    * CSS 在头部，JS 在尾部的优化（原理）

## 网络篇

* IP 地址转 INT
* 192.168.0.1/16 是什么意思
* DNS 主要作用是什么？
* IPv4 与 v6 区别

## 网络编程篇

* TCP 三次握手流程
* TCP、UDP 区别，分别适用场景
* 有什么办法能保证 UDP 高可用性(了解)
* TCP 粘包如何解决？
* 为什么需要心跳？
* 什么是长连接？
* HTTPS 是怎么保证安全的？
* 流与数据报的区别
* 进程间通信几种方式，最快的是哪种？
* fork 会发生什么？

## API 篇

* RESTful 是什么
* 如何在不支持 `DELETE` 请求的浏览器上兼容 `DELETE` 请求
* 常见的 app_id、app_secret 主要作用是什么？阐述下流程 
* API 请求如何保证数据不被篡改？
* JSON 和 JSONP 的区别
* 数据加密和验签的区别
* RSA 是什么
* API 版本兼容怎么处理
* 限流（木桶、令牌桶）
* OAuth 2 主要用在哪些场景下
* JWT
* PHP 中 `json_encode(['key'=>123]);` 与 `return json_encode([]);` 区别，会产生什么问题？如何解决

## 加分项
* 了解常用语言特性，及不同场景适用性。
   * PHP VS Golang
   * PHP VS Python
   * PHP VS JAVA
* 了解 PHP 扩展开发
* 熟练掌握 C


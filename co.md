

# 京东健康

1. Spring Boot 中Transaction / MySql中的事务？

Spring Boot 中的Transaction中有如下几个属性：read-only, rollback-for, no-robllback-for, timeout, progepation等。
需要熟悉各个属性的作用...
Trasaction 与 AOP 
(需要注意Transaction的自调用问题：在 Spring 的 AOP 代理下，只有目标方法由外部调用，目标方法才由 Spring 生成的代理对象来管理，这会造成自调用问题。若同一类中的其他没有@Transactional 注解的方法内部调用有@Transactional 注解的方法，有@Transactional 注解的方法的事务被忽略，不会发生回滚。解决方案，使用AspectJ 代替 Spring AOP)

2. 线程池

java.util.concurrent包中，使用Executors创建各种请情景下的线程类，其底层均是使用了原始的 ThreadPoolExecutor 创建线程, 主要三个参数coreSize, maximumPoolSize, workQueue.


3. 对象逃逸
  与之对应的是对象发布，也就是“将对象在当前作用域之外的地方被引用”,逃逸也便是再不该被发布的地方发布了，比如：在构造方法里面启动了调用了start()
  参照示例：https://app.yinxiang.com/shard/s11/nl/2273189/2123feeb-af34-424a-8b44-c4b6d2f5f052/

# 美团

1. 自定义string是否可以加载，如何加载？
2. 多线程问题
3. HashMap,HashTable,CocurrentHashMap
4. IOC / AOP
5. Bean 如何装配 
6. 双亲委派

# 小米
问了很多Why类问题



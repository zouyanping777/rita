# 1、@Pointcut
方法返回类型必须为void
execution 匹配方法执行的连接点

within 限定匹配特定类型的连接点

this 匹配特定链接点的bean引用是指定类型的实例的限制

target 限定匹配特点链接点的目标对象参数是指定类型的实例

args 限定匹配特点链接点的参数是给定类型的实例

@target 限定匹配特点链接点的类执行对象的具有给定类型的注解

@args 限定匹配特定连接点实际传入参数的类型具有给定类型的注解

@within 限定匹配到内具有给定的注释类型的连接点

@annotation 限定匹配特定连接点的主体具有给定的注解

代码：
<pre><code>
@Pointcut("execution(* com.imooc.aop.aspectj.biz.*Biz.*(..))")  
public void pointcut() {}  
      
@Pointcut("within(com.imooc.aop.aspectj.biz.*)")  
public void bizPointcut() {}  
</code></pre>

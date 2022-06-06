![core](core.png)
程序主要是通过Spring容器来访问容器中的Bean
依赖注入(IOC/DI)
Spring框架的核心功能有两个：
- Spring容器作为超级大工厂，负责创建、管理所有的Java对象，这些Java对象被称为Bean。
- Spring容器管理容器中Bean之间的依赖关系，Spring使用一种被称为"依赖注入"的方式来管理Bean之间的依赖关系。

设值注入
- 设值注入是指IoC容器通过成员变量的**setter方法**来注入被依赖对象。这种注入方式简单、直观，因而在Spring的依赖注入里大量使用。

构造注入
- 利用**构造器**来设置依赖关系的方式，被称为构造注入。通俗来说，就是驱动Spring在底层以反射方式执行带指定参数的构造器，当执行带参数的构造器时，就可利用构造器参数对成员变量执行初始化——这就是构造注入的本质。

### Bean
### Annotation
`@Required`: 它适用于 bean 设置方法。它指示必须在配置时使用必需的属性填充带注解的Bean，否则它将引发异常 BeanInitilizationException 。
`@Autowired`: : Spring通过提供@Autowired注解来提供基于注解的自动装配。它用于自动连接setter方法，实例变量和构造函数上的spring bean。当我们使用@Autowired批注时，spring容器通过匹配数据类型自动连接bean。
`@Configuration`: : 它是一个类级别的注解。带有@Configuration注解的类由Spring Containers用作bean定义的源。
`@ComponentScan`: : 当我们要扫描软件包中的bean时使用。它与注解@Configuration一起使用。我们还可以指定用于扫描Spring组件的基本软件包。
`@Bean`: 是方法级的注解。它是XML标记的代替方法。它告诉产生由Spring Container管理的bean的方法。
`@Component`: 。它是一个类级别的注解。它用于将Java类标记为Bean。在类路径中找到了一个用 @Component 注解的Java类。 Spring框架将其拾取并在应用程序上下文中将其配置为 Spring Bean 。
`@Controller`: @Controller是类级别的注解。它是 @Component 的专业化。它将一个类标记为Web请求处理程序。它通常用于服务网页。默认情况下，它返回一个字符串，该字符串指示要重定向的路由。它通常与 @RequestMapping 注解一起使用。
`@Service`: 也用于类级别。它告诉Spring该类包含 业务逻辑。
`@Repository`: 这是一个类级别的注解。该存储库是直接访问数据库的 DAO (数据访问对象)。该存储库执行与数据库有关的所有操作。
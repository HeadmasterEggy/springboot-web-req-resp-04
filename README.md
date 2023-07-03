| 注解          | 说明              | 位置                          |
|:------------|-----------------|-----------------------------|
| @Component  | 声明bean的基础注解     | 不属于以下三类时，用此注解               |
| @Controller | @Component的衍生注解 | 标注在控制器类上                    |
| @Service    | @Component的衍生注解 | 标注在业务类上                     |
| @Repository | @Component的衍生注解 | 标注在数据访问类上（由于与mybatis整合，用的少） |

**@Primary**

当存在多个相同类型的Bean注入时，加上@Primary注解，来确定默认的实现。


**@Qualifier**

指定当前要注入的bean对象。 在@Qualifier的value属性中，指定注入的bean的名称。
- @Qualifier注解不能单独使用，必须配合@Autowired使用

**@Resource**

是按照bean的名称进行注入。通过name属性指定要注入的bean的名称。
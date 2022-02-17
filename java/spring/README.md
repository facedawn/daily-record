# @Transactional 

用于回滚使用的注解。

在启动类上添加@EnableTransactionManagement注解。

@Transactional(readOnly = true, rollbackFor = Exception.class)，那么被注解修饰的类中的方法抛出异常时，就会回滚。

如果不配置rollbackFor属性,那么事物只会在遇到RuntimeException的时候才会回滚,加上rollbackFor=Exception.class,可以让事物在遇到非运行时异常时也回滚。

# @Api系列注解
是swagger里的

注解@ApiOperation是用来构建Api文档的

@ApiOperation(value = “接口说明”, httpMethod = “接口请求方式”, response =“接口返回参数类型”, notes = “接口发布说明”；

@Api：用在请求的类上，表示对类的说明，tags="说明该类的作用，可以在UI界面上看到的注解"

@ApiImplicitParams：用在请求的方法上，表示一组参数说明

@ApiImplicitParam：用在@ApiImplicitParams注解中，指定一个请求参数的各个方面

@ApiResponses：用在请求的方法上，表示一组响应

@ApiResponse：用在@ApiResponses中，一般用于表达一个错误的响应信息
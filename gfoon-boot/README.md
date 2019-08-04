
### gfoon-boot框架说明 
#### 工程项目结构

|          工程名称                                                | 工程说明 |
|        ----------------------------------------------          |----------------------|
|gfoon-boot                                                      | 脚手架父级POM工程 |
|│......gfoon-boot-bi                                            | 业务逻辑父级POM工程|
|│......│......gfoon-boot-bi-xxx                                 | xxx业务逻辑POM工程|
|│......│......│......gfoon-boot-bi-xxx-dao                      | 业务数据接口服务层（DO、Dao）|
|│......│......│......gfoon-boot-bi-xxx-dao                      | 业务实体类（VO、DTO、PO）|
|│......│......│......gfoon-boot-bi-xxx-dao                      | 业务逻辑处理层(Service、Impl)|
|│......│......│......gfoon-boot-bi-xxx-dao                      | 业务视图控制层及Rest接口（Controller/Api）|
|│......gfoon-boot-cloud                                         | 微服务分布式服务父级工程|
|│......│......gfoon-boot-cloud-bus                              | 消息总线|
|│......│......gfoon-boot-cloud-config                           | 云端配置中心|
|│......│......gfoon-boot-cloud-eureka                           | 服务注册中心|
|│......│......gfoon-boot-cloud-dubbo                            | dubbo分布式服务|
|│......│......gfoon-boot-cloud-feign                            | 声明式、模板化客户端，优雅调用HTTP API|
|│......│......gfoon-boot-cloud-gateway                          | API网关|
|│......│......gfoon-boot-cloud-hystrix                          | 断路器|
|│......│......gfoon-boot-cloud-ribbon                           | 负载均衡|
|│......│......gfoon-boot-cloud-stream                           | 消息队列|
|│......│......gfoon-boot-cloud-sleuth                           | 服务链路追踪|
|│......gfoon-boot-sys                                           | 系统核心服务父级工程|
|│......│......gfoon-boot-sys-actuator                           | 服务监控|
|│......│......gfoon-boot-sys-admin                              | springBoot 监控平台|
|│......│......gfoon-boot-sys-common                             | 通用工具类服务|
|│......│......gfoon-boot-sys-config                             | 配置文件服务|
|│......│......gfoon-boot-sys-core                               | 核心类封装|
|│......│......gfoon-boot-sys-durid                              | 数据库监控|
|│......│......gfoon-boot-sys-fileio                             | 文件相关操作|
|│......│......gfoon-boot-sys-permission                         | 权限实现层服务|
|│......│......gfoon-boot-sys-plugins                            | 插件服务，UI插件|
|│......│......gfoon-boot-sys-pojo                               | 系统权限的实体类|
|│......│......gfoon-boot-sys-security                           | 安全拦截服务|
|│......│......gfoon-boot-sys-swagger                            | 接口文档自动生成服务|
|│......│......gfoon-boot-sys-web                                | 系统管理后台 |
|│......gfoon-boot-web                                           | 业务web服务|
|│......│......gfoon-boot-web-xxx                                | xxx业务展现（MiniUI、VUE等）|
                  
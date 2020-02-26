spring/spring boot/spring cloud注解整理
--------------------------------------


## spring

#### 收集命令

```bash

cd spring-framework

for p in `ls | grep spring`; do echo "- - #### $p"; for i in `find $p`; do grep '^public @interface' $i 2> err_out; done; done

```

#### spring-aop

Tx 
EmptySpringAnnotation 

#### spring-aspects

EnableSpringConfigured 

#### spring-beans

TestAnnotation 
Lookup 
Required 
Configurable 
Qualifier 
Value 
Autowired 

#### spring-context

MyRepository 
BeanAge 
Log 
MyScope 
CustomComponent 
CustomStereotype 
CustomAspectStereotype 
DevComponent 
Profile 
PropertySource 
PropertySources 
DependsOn 
ComponentScan 
ComponentScans 
EnableLoadTimeWeaving 
Configuration 
EnableMBeanExport 
Description 
Lazy 
EnableAspectJAutoProxy 
Import 
Primary 
Scope 
Bean 
Role 
ImportResource 
Conditional 
EventListener 
Caching 
CacheEvict 
CachePut 
CacheConfig 
Cacheable 
EnableCaching 
Async 
EnableAsync 
Schedules 
EnableScheduling 
Scheduled 
ManagedAttribute 
ManagedOperationParameters 
ManagedMetric 
ManagedNotifications 
ManagedResource 
ManagedOperation 
ManagedOperationParameter 
ManagedNotification 
Component 
Controller 
Service 
Repository 
Indexed 
NumberFormat 
DateTimeFormat 
Validated 

#### spring-context-indexer

MetaControllerIndexed 
MetaController 

#### spring-context-support

#### spring-core

TestQualifier 
TestAutowired 
Scope 
EnabledForTestGroups 
Component 
Indexed 
NonInheritedAnnotation 
InheritedAnnotation 
Order 
AliasFor 
NonNull 
NonNullApi 
UsesSunHttpServer 
UsesJava7 
UsesJava8 
UsesSunMisc 
NonNullFields 
Nullable 

#### spring-expression
#### spring-framework-bom
#### spring-instrument
#### spring-jcl
#### spring-jdbc
#### spring-jms

EnableJms 
JmsListener 
JmsListeners 

#### spring-messaging

<span class="memberNameLabel">MessageMapping</span></pre>
<span class="memberNameLabel">Payload</span></pre>
<span class="memberNameLabel">MessageExceptionHandler</span></pre>
<span class="memberNameLabel">DestinationVariable</span></pre>
<span class="memberNameLabel">Headers</span></pre>
<span class="memberNameLabel">SendTo</span></pre>
<span class="memberNameLabel">Header</span></pre>
<span class="memberNameLabel">SubscribeMapping</span></pre>
<span class="memberNameLabel">SendToUser</span></pre>
MessageMapping 
Payload 
MessageExceptionHandler 
DestinationVariable 
Headers 
SendTo 
Header 
SubscribeMapping 
SendToUser 
ConnectMapping 

#### spring-orm
#### spring-oxm
#### spring-test

MetaMetaContextHierarchyConfig 
MetaContextHierarchyConfig 
FailingTestCase 
DisabledOnMac 
EnabledOnMac 
WebTestConfiguration 
ConfigClassesAndProfileResolverWithCustomDefaultsMetaConfig 
ConfigClassesAndProfilesWithCustomDefaultsMetaConfig 
ConfigClassesAndProfilesMetaConfig 
MetaMetaConfig 
TestExecutionListeners 
AfterTransaction 
BeforeTransaction 
TestConstructor 
SpringJUnitConfig 
SpringJUnitWebConfig 
DisabledIf 
EnabledIf 
WebAppConfiguration 
ContextHierarchy 
BootstrapWith 
SqlMergeMode 
SqlConfig 
Sql 
SqlGroup 
TestPropertySource 
ContextConfiguration 
TestPropertySources 
ActiveProfiles 
BeforeTestMethod 
AfterTestClass 
AfterTestMethod 
BeforeTestClass 
AfterTestExecution 
PrepareTestInstance 
BeforeTestExecution 
DirtiesContext 
Repeat 
ProfileValueSourceConfiguration 
Timed 
Commit 
Rollback 
IfProfileValue 

#### spring-tx

NoSynch 
EnableTransactionManagement 
Transactional 
TransactionalEventListener 

#### spring-web

RequestScope 
SessionScope 
ApplicationScope 
DeleteMapping 
PostMapping 
ExceptionHandler 
RequestHeader 
CrossOrigin 
RestControllerAdvice 
ResponseStatus 
PathVariable 
RequestAttribute 
ResponseBody 
RequestParam 
SessionAttribute 
ControllerAdvice 
Mapping 
SessionAttributes 
RequestMapping 
RequestBody 
PutMapping 
RequestPart 
MatrixVariable 
InitBinder 
CookieValue 
RestController 
PatchMapping 
GetMapping 
ModelAttribute 

#### spring-webflux

EnableWebFlux 

#### spring-webmvc

EnableWebMvc 

#### spring-websocket

EnableWebSocketMessageBroker 
EnableWebSocket 


## spring boot

#### spring-boot

MetaComponentScan 
SpringBootConfiguration 
DeprecatedConfigurationProperty 
ConfigurationProperties 
EnableConfigurationProperties 
NestedConfigurationProperty 
ConstructorBinding 
ConfigurationPropertiesScan 
DefaultValue 
ConfigurationPropertiesBinding 
ServletComponentScan 
LocalServerPort 
LocalRSocketServerPort 
DurationUnit 
DataSizeUnit 
Delimiter 
DurationFormat 
JsonComponent 

#### spring-boot-actuator

WebEndpointTest 
EndpointWebExtension 
WebEndpoint 
ServletEndpoint 
RestControllerEndpoint 
ControllerEndpoint 
JmxEndpoint 
EndpointJmxExtension 
EndpointExtension 
ReadOperation 
Endpoint 
Selector 
EndpointConverter 
WriteOperation 
FilteredEndpoint 
DeleteOperation 

#### spring-boot-actuator-autoconfigure

LocalManagementPort 
ConditionalOnManagementPort 
ManagementContextConfiguration 
EndpointCloudFoundryExtension 
ConditionalOnEnabledHealthIndicator 
ConditionalOnEnabledInfoContributor 
ConditionalOnAvailableEndpoint 
ConditionalOnEnabledEndpoint 

#### spring-boot-autoconfigure

TestAutoConfigurationPackage 
ImportAutoConfiguration 
ConditionalOnMissingFilterBean 
ConditionalOnEnabledResourceChain 
AutoConfigureAfter 
AutoConfigurationPackage 
AutoConfigureBefore 
ConditionalOnCloudPlatform 
ConditionalOnJndi 
ConditionalOnNotWebApplication 
ConditionalOnExpression 
ConditionalOnJava 
ConditionalOnMissingBean 
ConditionalOnWebApplication 
ConditionalOnResource 
ConditionalOnSingleCandidate 
ConditionalOnMissingClass 
ConditionalOnProperty 
ConditionalOnClass 
ConditionalOnBean 
SpringBootApplication 
BatchDataSource 
EnableAutoConfiguration 
QuartzDataSource 
LiquibaseDataSource 
ConditionalOnRepositoryType 
AutoConfigureOrder 
EntityScan 
FlywayDataSource 

#### spring-boot-cli

DependencyManagementBom 
EnableGroovyTemplates 

#### spring-boot-dependencies
#### spring-boot-devtools

ConditionalOnInitializedRestarter 
RestartScope 

#### spring-boot-docs
#### spring-boot-parent
#### spring-boot-project.iml
#### spring-boot-properties-migrator
#### spring-boot-starters

#### spring-boot-test

CustomQualifier 
SpringBootTest 
TestConfiguration 
TestComponent 
SpyBeans 
MockBean 
SpyBean 
MockBeans 

#### spring-boot-test-autoconfigure

JooqTest 
AutoConfigureJooq 
AutoConfigureCache 
AutoConfigureMockMvc 
WebMvcTest 
AutoConfigureWebMvc 
AutoConfigureWebFlux 
WebFluxTest 
AutoConfigureWebTestClient 
RestClientTest 
AutoConfigureWebClient 
AutoConfigureMockRestServiceServer 
JdbcTest 
AutoConfigureTestDatabase 
AutoConfigureJdbc 
AutoConfigureJsonTesters 
JsonTest 
AutoConfigureJson 
PropertyMapping 
OverrideAutoConfiguration 
DataJpaTest 
AutoConfigureDataJpa 
AutoConfigureTestEntityManager 
TypeExcludeFilters 
AutoConfigureDataNeo4j 
DataNeo4jTest 
AutoConfigureDataRedis 
DataRedisTest 
AutoConfigureDataLdap 
DataLdapTest 
DataJdbcTest 
AutoConfigureDataJdbc 
AutoConfigureDataMongo 
DataMongoTest 
AutoConfigureRestDocs 

#### spring-boot-tools

TestAutoConfigureAfter 
TestConditionalOnSingleCandidate 
TestConditionalOnWebApplication 
TestConditionalOnClass 
TestAutoConfigureBefore 
TestAutoConfigureOrder 
TestConditionalOnBean 
ClassPathOverrides 
ClassPathExclusions 
DeprecatedConfigurationProperty 
MetaConstructorBinding 
ReadOperation 
ConfigurationProperties 
NestedConfigurationProperty 
MetaEndpoint 
Endpoint 
DefaultValue 
ConstructorBinding 




## spring cloud

### spring-cloud-commons

#### spring-cloud-commons

ConditionalOnDiscoveryHealthIndicatorEnabled 
SpringCloudApplication 
EnableDiscoveryClient 
LoadBalanced 
EnableCircuitBreaker 
ConditionalOnBlockingDiscoveryEnabled 
ConditionalOnDiscoveryEnabled 
ConditionalOnReactiveDiscoveryEnabled 


#### spring-cloud-commons-dependencies

#### spring-cloud-commons-parent.iml

#### spring-cloud-context

RefreshScope 
BootstrapConfiguration 

#### spring-cloud-context-integration-tests

#### spring-cloud-loadbalancer

LoadBalancerClient 
LoadBalancerClients 

#### spring-cloud-starter

#### spring-cloud-starter-loadbalancer

#### spring-cloud-test-support

ClassPathOverrides 
ClassPathExclusions 



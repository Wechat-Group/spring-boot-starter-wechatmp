spring-boot-start-wechatmp
===================================
Spring Boot对微信公众号(订阅号、服务号)的支持

### usage
in pom.xml add following dependency:

      <dependency>
          <groupId>org.mvnsearch.wechat</groupId>
          <artifactId>spring-boot-starter-wechatmp</artifactId>
          <version>0.0.1-SNAPSHOT</version>
      </dependency>
      
in application.properties file, please add following keys:

     spring.wechatmp.appId=xxxx
     spring.wechatmp.secret=yyyy
     spring.wechatmp.token=xxx-dev
     spring.wechatmp.aesKey=xxx-dev
     
in your code you can use OssClient directly:

     @Autowired
     WxMpService wxMpService;
     
### spring-boot-start-wechatmp service List

* me.chanjar.weixin.mp.api.WxMpInMemoryConfigStorage: config storage
* me.chanjar.weixin.mp.api.WxMpService: wechat MP service

### 参考

* wechat开发文档: https://github.com/chanjarster/weixin-java-tools/wiki
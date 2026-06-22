# zheng

## Summary

| Metric | Value |
|--------|-------|
| Total Issues | 114 |
| Mandatory Blockers | 99 |
| Potential Issues | 7 |

## Component Information

| Property | Value |
|----------|-------|
| Language | Java, JavaScript |
| Frameworks | Spring |
| Build tools | Maven |
| JDK version | 1.7 |

## Cloud Readiness Issues

| Issue Name | Criticality | Story Points | Occurrences |
|------------|-------------|--------------|-------------|
| Avoid File System Logging in Configuration | Mandatory | 1 | [76](#Avoid_File_System_Logging_in_Configuration) |
| Use of unsecured network protocols or URI libraries | Mandatory | 3 | [59](#Use_of_unsecured_network_protocols_or_URI_libraries) |
| CRA: Hard-coded credentials in configuration files | Mandatory | 5 | [38](#CRA_Hard-coded_credentials_in_configuration_files) |
| CRA: Hard-coded password in Java source code | Mandatory | 8 | [3](#CRA_Hard-coded_password_in_Java_source_code) |
| CRA: Use of insecure random number generator java.util.Random | Mandatory | 5 | [2](#CRA_Use_of_insecure_random_number_generator_java_util_Random) |
| CRA: Default or well-known password detected | Mandatory | 3 | [2](#CRA_Default_or_well-known_password_detected) |
| Hardcoded IP Address | Mandatory | 3 | [2](#Hardcoded_IP_Address) |
| No Dockerfile found | Mandatory | 3 | 1 |
| Local HTTP Calls | Mandatory | 3 | [1](#Local_HTTP_Calls) |
| CRA: Use of weak hash algorithm MD5 | Mandatory | 5 | [1](#CRA_Use_of_weak_hash_algorithm_MD5) |
| ActiveMQ found | Potential | 5 | [5](#ActiveMQ_found) |
| CRA: Use of Math.random() which is not cryptographically secure | Potential | 3 | [1](#CRA_Use_of_Math_random_which_is_not_cryptographically_secure) |
| Avoid using hardcoded URLs (HTTP protocol) in source code | Optional | 3 | [59](#Avoid_using_hardcoded_URLs_HTTP_protocol_in_source_code) |
| Localhost Usage | Optional | 3 | [8](#Localhost_Usage) |

### Issue Details

<details id="Avoid_File_System_Logging_in_Configuration">
<summary><b>Avoid File System Logging in Configuration</b> — affected files</summary>

- `zheng-wechat/zheng-wechat-mp/zheng-wechat-mp-admin/src/main/resources/log4j.properties (line 12)`
- `zheng-wechat/zheng-wechat-mp/zheng-wechat-mp-admin/src/main/resources/log4j.properties (line 13)`
- `zheng-wechat/zheng-wechat-mp/zheng-wechat-mp-admin/src/main/resources/log4j.properties (line 21)`
- `zheng-wechat/zheng-wechat-mp/zheng-wechat-mp-admin/src/main/resources/log4j.properties (line 22)`
- `zheng-api/zheng-api-rpc-service/src/main/resources/log4j.properties (line 12)`
- `zheng-api/zheng-api-rpc-service/src/main/resources/log4j.properties (line 13)`
- `zheng-api/zheng-api-rpc-service/src/main/resources/log4j.properties (line 21)`
- `zheng-api/zheng-api-rpc-service/src/main/resources/log4j.properties (line 22)`
- `zheng-api/zheng-api-server/src/main/resources/log4j.properties (line 12)`
- `zheng-api/zheng-api-server/src/main/resources/log4j.properties (line 13)`
- `zheng-api/zheng-api-server/src/main/resources/log4j.properties (line 21)`
- `zheng-api/zheng-api-server/src/main/resources/log4j.properties (line 22)`
- `zheng-cms/zheng-cms-admin/src/main/resources/log4j.properties (line 12)`
- `zheng-cms/zheng-cms-admin/src/main/resources/log4j.properties (line 13)`
- `zheng-cms/zheng-cms-admin/src/main/resources/log4j.properties (line 21)`
- `zheng-cms/zheng-cms-admin/src/main/resources/log4j.properties (line 22)`
- `zheng-cms/zheng-cms-job/src/main/resources/log4j.properties (line 12)`
- `zheng-cms/zheng-cms-job/src/main/resources/log4j.properties (line 13)`
- `zheng-cms/zheng-cms-job/src/main/resources/log4j.properties (line 21)`
- `zheng-cms/zheng-cms-job/src/main/resources/log4j.properties (line 22)`
- `zheng-pay/zheng-pay-rpc-service/src/main/resources/log4j.properties (line 12)`
- `zheng-pay/zheng-pay-rpc-service/src/main/resources/log4j.properties (line 13)`
- `zheng-pay/zheng-pay-rpc-service/src/main/resources/log4j.properties (line 21)`
- `zheng-pay/zheng-pay-rpc-service/src/main/resources/log4j.properties (line 22)`
- `zheng-pay/zheng-pay-web/src/main/resources/log4j.properties (line 12)`
- `zheng-pay/zheng-pay-web/src/main/resources/log4j.properties (line 13)`
- `zheng-pay/zheng-pay-web/src/main/resources/log4j.properties (line 21)`
- `zheng-pay/zheng-pay-web/src/main/resources/log4j.properties (line 22)`
- `zheng-ucenter/zheng-ucenter-rpc-service/src/main/resources/log4j.properties (line 12)`
- `zheng-ucenter/zheng-ucenter-rpc-service/src/main/resources/log4j.properties (line 13)`
- `zheng-ucenter/zheng-ucenter-rpc-service/src/main/resources/log4j.properties (line 21)`
- `zheng-ucenter/zheng-ucenter-rpc-service/src/main/resources/log4j.properties (line 22)`
- `zheng-ucenter/zheng-ucenter-web/src/main/resources/log4j.properties (line 12)`
- `zheng-ucenter/zheng-ucenter-web/src/main/resources/log4j.properties (line 13)`
- `zheng-ucenter/zheng-ucenter-web/src/main/resources/log4j.properties (line 21)`
- `zheng-ucenter/zheng-ucenter-web/src/main/resources/log4j.properties (line 22)`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/log4j.properties (line 12)`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/log4j.properties (line 13)`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/log4j.properties (line 21)`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/log4j.properties (line 22)`
- `zheng-upms/zheng-upms-server/src/main/resources/log4j.properties (line 12)`
- `zheng-upms/zheng-upms-server/src/main/resources/log4j.properties (line 13)`
- `zheng-upms/zheng-upms-server/src/main/resources/log4j.properties (line 21)`
- `zheng-upms/zheng-upms-server/src/main/resources/log4j.properties (line 22)`
- `zheng-demo/zheng-demo-web/src/main/resources/log4j.properties (line 12)`
- `zheng-demo/zheng-demo-web/src/main/resources/log4j.properties (line 13)`
- `zheng-demo/zheng-demo-web/src/main/resources/log4j.properties (line 21)`
- `zheng-demo/zheng-demo-web/src/main/resources/log4j.properties (line 22)`
- `zheng-message/zheng-message-server/src/main/resources/log4j.properties (line 12)`
- `zheng-message/zheng-message-server/src/main/resources/log4j.properties (line 13)`
- `zheng-message/zheng-message-server/src/main/resources/log4j.properties (line 21)`
- `zheng-message/zheng-message-server/src/main/resources/log4j.properties (line 22)`
- `zheng-oss/zheng-oss-admin/src/main/resources/log4j.properties (line 12)`
- `zheng-oss/zheng-oss-admin/src/main/resources/log4j.properties (line 13)`
- `zheng-oss/zheng-oss-admin/src/main/resources/log4j.properties (line 21)`
- `zheng-oss/zheng-oss-admin/src/main/resources/log4j.properties (line 22)`
- `zheng-oss/zheng-oss-web/src/main/resources/log4j.properties (line 12)`
- `zheng-oss/zheng-oss-web/src/main/resources/log4j.properties (line 13)`
- `zheng-oss/zheng-oss-web/src/main/resources/log4j.properties (line 21)`
- `zheng-oss/zheng-oss-web/src/main/resources/log4j.properties (line 22)`
- `zheng-pay/zheng-pay-admin/src/main/resources/log4j.properties (line 12)`
- `zheng-pay/zheng-pay-admin/src/main/resources/log4j.properties (line 13)`
- `zheng-pay/zheng-pay-admin/src/main/resources/log4j.properties (line 21)`
- `zheng-pay/zheng-pay-admin/src/main/resources/log4j.properties (line 22)`
- `zheng-cms/zheng-cms-web/src/main/resources/log4j.properties (line 12)`
- `zheng-cms/zheng-cms-web/src/main/resources/log4j.properties (line 13)`
- `zheng-cms/zheng-cms-web/src/main/resources/log4j.properties (line 21)`
- `zheng-cms/zheng-cms-web/src/main/resources/log4j.properties (line 22)`
- `zheng-cms/zheng-cms-rpc-service/src/main/resources/log4j.properties (line 12)`
- `zheng-cms/zheng-cms-rpc-service/src/main/resources/log4j.properties (line 13)`
- `zheng-cms/zheng-cms-rpc-service/src/main/resources/log4j.properties (line 21)`
- `zheng-cms/zheng-cms-rpc-service/src/main/resources/log4j.properties (line 22)`
- `zheng-cms/zheng-cms-search/src/main/resources/log4j.properties (line 12)`
- `zheng-cms/zheng-cms-search/src/main/resources/log4j.properties (line 13)`
- `zheng-cms/zheng-cms-search/src/main/resources/log4j.properties (line 21)`
- `zheng-cms/zheng-cms-search/src/main/resources/log4j.properties (line 22)`

</details>

<details id="Use_of_unsecured_network_protocols_or_URI_libraries">
<summary><b>Use of unsecured network protocols or URI libraries</b> — affected files</summary>

- `zheng-oss/zheng-oss-web/src/main/java/com/zheng/oss/web/controller/AliyunOssController.java (line 58)`
- `zheng-oss/zheng-oss-web/src/main/java/com/zheng/oss/web/controller/DemoController.java (line 71)`
- `zheng-oss/zheng-oss-web/src/main/java/com/zheng/oss/web/service/AliyunOssService.java (line 49)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/dev.properties (line 3)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/dev.properties (line 13)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/dev.properties (line 16)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/prod.properties (line 3)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/prod.properties (line 13)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/prod.properties (line 16)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/test.properties (line 3)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/test.properties (line 13)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/test.properties (line 16)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/dev.properties (line 12)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/dev.properties (line 13)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/dev.properties (line 16)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/prod.properties (line 12)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/prod.properties (line 13)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/prod.properties (line 16)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/test.properties (line 12)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/test.properties (line 13)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/test.properties (line 16)`
- `zheng-ucenter/zheng-ucenter-web/src/main/resources/profiles/dev.properties (line 3)`
- `zheng-ucenter/zheng-ucenter-web/src/main/resources/profiles/prod.properties (line 3)`
- `zheng-ucenter/zheng-ucenter-web/src/main/resources/profiles/test.properties (line 3)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/dev.properties (line 17)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/dev.properties (line 27)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/dev.properties (line 36)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/test.properties (line 17)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/test.properties (line 27)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/test.properties (line 36)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/prod.properties (line 17)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/prod.properties (line 27)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/prod.properties (line 36)`
- `zheng-cms/zheng-cms-admin/src/main/resources/profiles/dev.properties (line 27)`
- `zheng-cms/zheng-cms-admin/src/main/resources/profiles/dev.properties (line 39)`
- `zheng-cms/zheng-cms-admin/src/main/resources/profiles/prod.properties (line 27)`
- `zheng-cms/zheng-cms-admin/src/main/resources/profiles/prod.properties (line 39)`
- `zheng-cms/zheng-cms-admin/src/main/resources/profiles/test.properties (line 27)`
- `zheng-cms/zheng-cms-admin/src/main/resources/profiles/test.properties (line 39)`
- `zheng-cms/zheng-cms-web/src/main/resources/profiles/dev.properties (line 3)`
- `zheng-cms/zheng-cms-web/src/main/resources/profiles/prod.properties (line 3)`
- `zheng-cms/zheng-cms-web/src/main/resources/profiles/test.properties (line 3)`
- `zheng-demo/zheng-demo-web/src/main/java/com/zheng/demo/web/controller/IndexController.java (line 45)`
- `zheng-demo/zheng-demo-web/src/main/resources/profiles/dev.properties (line 3)`
- `zheng-demo/zheng-demo-web/src/main/resources/profiles/dev.properties (line 9)`
- `zheng-demo/zheng-demo-web/src/main/resources/profiles/prod.properties (line 3)`
- `zheng-demo/zheng-demo-web/src/main/resources/profiles/prod.properties (line 9)`
- `zheng-demo/zheng-demo-web/src/main/resources/profiles/test.properties (line 3)`
- `zheng-demo/zheng-demo-web/src/main/resources/profiles/test.properties (line 9)`
- `zheng-message/zheng-message-sdk/src/main/java/com/zheng/message/sdk/MessageHelper.java (line 58)`
- `zheng-message/zheng-message-server/src/main/resources/profiles/dev.properties (line 3)`
- `zheng-message/zheng-message-server/src/main/resources/profiles/prod.properties (line 3)`
- `zheng-message/zheng-message-server/src/main/resources/profiles/test.properties (line 3)`
- `zheng-oss/zheng-oss-admin/src/main/resources/profiles/dev.properties (line 22)`
- `zheng-oss/zheng-oss-admin/src/main/resources/profiles/prod.properties (line 22)`
- `zheng-oss/zheng-oss-admin/src/main/resources/profiles/test.properties (line 22)`
- `zheng-api/zheng-api-server/src/main/resources/profiles/dev.properties (line 18)`
- `zheng-api/zheng-api-server/src/main/resources/profiles/prod.properties (line 18)`
- `zheng-api/zheng-api-server/src/main/resources/profiles/test.properties (line 18)`

</details>

<details id="CRA_Hard-coded_credentials_in_configuration_files">
<summary><b>CRA: Hard-coded credentials in configuration files</b> — affected files</summary>

- `zheng-cms/zheng-cms-dao/src/main/resources/generator.properties (line 4)`
- `zheng-cms/zheng-cms-rpc-service/src/main/resources/jdbc.properties (line 4)`
- `zheng-cms/zheng-cms-rpc-service/src/main/resources/jdbc.properties (line 8)`
- `zheng-cms/zheng-cms-rpc-service/src/main/resources/profiles/dev.properties (line 8)`
- `zheng-cms/zheng-cms-rpc-service/src/main/resources/profiles/dev.properties (line 12)`
- `zheng-cms/zheng-cms-rpc-service/src/main/resources/profiles/prod.properties (line 8)`
- `zheng-cms/zheng-cms-rpc-service/src/main/resources/profiles/prod.properties (line 12)`
- `zheng-cms/zheng-cms-rpc-service/src/main/resources/profiles/test.properties (line 8)`
- `zheng-cms/zheng-cms-rpc-service/src/main/resources/profiles/test.properties (line 12)`
- `zheng-pay/zheng-pay-dao/src/main/resources/generator.properties (line 4)`
- `zheng-pay/zheng-pay-rpc-service/src/main/resources/jdbc.properties (line 4)`
- `zheng-pay/zheng-pay-rpc-service/src/main/resources/jdbc.properties (line 8)`
- `zheng-pay/zheng-pay-rpc-service/src/main/resources/profiles/dev.properties (line 8)`
- `zheng-pay/zheng-pay-rpc-service/src/main/resources/profiles/dev.properties (line 12)`
- `zheng-pay/zheng-pay-rpc-service/src/main/resources/profiles/prod.properties (line 8)`
- `zheng-pay/zheng-pay-rpc-service/src/main/resources/profiles/prod.properties (line 12)`
- `zheng-pay/zheng-pay-rpc-service/src/main/resources/profiles/test.properties (line 8)`
- `zheng-pay/zheng-pay-rpc-service/src/main/resources/profiles/test.properties (line 12)`
- `zheng-ucenter/zheng-ucenter-dao/src/main/resources/generator.properties (line 4)`
- `zheng-ucenter/zheng-ucenter-rpc-service/src/main/resources/jdbc.properties (line 4)`
- `zheng-ucenter/zheng-ucenter-rpc-service/src/main/resources/jdbc.properties (line 8)`
- `zheng-ucenter/zheng-ucenter-rpc-service/src/main/resources/profiles/dev.properties (line 8)`
- `zheng-ucenter/zheng-ucenter-rpc-service/src/main/resources/profiles/dev.properties (line 12)`
- `zheng-ucenter/zheng-ucenter-rpc-service/src/main/resources/profiles/prod.properties (line 8)`
- `zheng-ucenter/zheng-ucenter-rpc-service/src/main/resources/profiles/prod.properties (line 12)`
- `zheng-ucenter/zheng-ucenter-rpc-service/src/main/resources/profiles/test.properties (line 8)`
- `zheng-ucenter/zheng-ucenter-rpc-service/src/main/resources/profiles/test.properties (line 12)`
- `zheng-upms/zheng-upms-dao/src/main/resources/generator.properties (line 4)`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/jdbc.properties (line 4)`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/jdbc.properties (line 8)`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/profiles/dev.properties (line 8)`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/profiles/dev.properties (line 12)`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/profiles/prod.properties (line 8)`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/profiles/prod.properties (line 12)`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/profiles/test.properties (line 8)`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/profiles/test.properties (line 12)`
- `zheng-wechat/zheng-wechat-mp/zheng-wechat-mp-dao/src/main/resources/jdbc.properties (line 4)`
- `zheng-wechat/zheng-wechat-mp/zheng-wechat-mp-dao/src/main/resources/jdbc.properties (line 8)`

</details>

<details id="CRA_Hard-coded_password_in_Java_source_code">
<summary><b>CRA: Hard-coded password in Java source code</b> — affected files</summary>

- `zheng-ucenter/zheng-ucenter-dao/src/main/java/com/zheng/ucenter/dao/model/UcenterUserExample.java (line 182)`
- `zheng-upms/zheng-upms-dao/src/main/java/com/zheng/upms/dao/model/UpmsUserExample.java (line 251)`
- `zheng-upms/zheng-upms-rpc-service/src/test/java/com/zheng/upms/rpc/service/UpmsServiceTest.java (line 49)`

</details>

<details id="CRA_Use_of_insecure_random_number_generator_java_util_Random">
<summary><b>CRA: Use of insecure random number generator java.util.Random</b> — affected files</summary>

- `zheng-common/src/main/java/com/zheng/common/util/CaptchaUtil.java (line 27)`
- `zheng-common/src/main/java/com/zheng/common/util/CaptchaUtil.java (line 139)`

</details>

<details id="CRA_Default_or_well-known_password_detected">
<summary><b>CRA: Default or well-known password detected</b> — affected files</summary>

- `zheng-ucenter/zheng-ucenter-dao/src/main/java/com/zheng/ucenter/dao/model/UcenterUser.java (line 92)`
- `zheng-upms/zheng-upms-dao/src/main/java/com/zheng/upms/dao/model/UpmsUser.java (line 106)`

</details>

<details id="Hardcoded_IP_Address">
<summary><b>Hardcoded IP Address</b> — affected files</summary>

- `zheng-cms/zheng-cms-web/src/main/java/com/zheng/cms/web/rocketmq/Consumer.java (line 21)`
- `zheng-cms/zheng-cms-web/src/main/java/com/zheng/cms/web/rocketmq/Producer.java (line 14)`

</details>

<details id="Local_HTTP_Calls">
<summary><b>Local HTTP Calls</b> — affected files</summary>

- `zheng-message/zheng-message-sdk/src/main/java/com/zheng/message/sdk/MessageHelper.java (line 58)`

</details>

<details id="CRA_Use_of_weak_hash_algorithm_MD5">
<summary><b>CRA: Use of weak hash algorithm MD5</b> — affected files</summary>

- `zheng-common/src/main/java/com/zheng/common/util/MD5Util.java (line 20)`

</details>

<details id="ActiveMQ_found">
<summary><b>ActiveMQ found</b> — affected files</summary>

- `project-tools/activemq.bat.lnk`
- `zheng-api/zheng-api-server/src/main/resources/applicationContext-activemq.xml`
- `zheng-cms/zheng-cms-admin/src/main/resources/applicationContext-activemq.xml`
- `zheng-cms/zheng-cms-job/src/main/resources/applicationContext-activemq.xml`
- `zheng-cms/zheng-cms-web/src/main/resources/applicationContext-activemq.xml`

</details>

<details id="CRA_Use_of_Math_random_which_is_not_cryptographically_secure">
<summary><b>CRA: Use of Math.random() which is not cryptographically secure</b> — affected files</summary>

- `zheng-common/src/main/java/com/zheng/common/util/CaptchaUtil.java (line 115)`

</details>

<details id="Avoid_using_hardcoded_URLs_HTTP_protocol_in_source_code">
<summary><b>Avoid using hardcoded URLs (HTTP protocol) in source code</b> — affected files</summary>

- `zheng-oss/zheng-oss-web/src/main/resources/profiles/dev.properties (line 3)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/dev.properties (line 13)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/dev.properties (line 16)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/prod.properties (line 3)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/prod.properties (line 13)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/prod.properties (line 16)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/test.properties (line 3)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/test.properties (line 13)`
- `zheng-oss/zheng-oss-web/src/main/resources/profiles/test.properties (line 16)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/dev.properties (line 5)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/dev.properties (line 12)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/dev.properties (line 13)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/dev.properties (line 16)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/prod.properties (line 5)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/prod.properties (line 12)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/prod.properties (line 13)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/prod.properties (line 16)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/test.properties (line 5)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/test.properties (line 12)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/test.properties (line 13)`
- `zheng-pay/zheng-pay-web/src/main/resources/profiles/test.properties (line 16)`
- `zheng-ucenter/zheng-ucenter-web/src/main/resources/profiles/dev.properties (line 3)`
- `zheng-ucenter/zheng-ucenter-web/src/main/resources/profiles/prod.properties (line 3)`
- `zheng-ucenter/zheng-ucenter-web/src/main/resources/profiles/test.properties (line 3)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/dev.properties (line 17)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/dev.properties (line 27)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/dev.properties (line 36)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/prod.properties (line 17)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/prod.properties (line 27)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/prod.properties (line 36)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/test.properties (line 17)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/test.properties (line 27)`
- `zheng-upms/zheng-upms-server/src/main/resources/profiles/test.properties (line 36)`
- `zheng-api/zheng-api-server/src/main/resources/profiles/dev.properties (line 18)`
- `zheng-api/zheng-api-server/src/main/resources/profiles/prod.properties (line 18)`
- `zheng-api/zheng-api-server/src/main/resources/profiles/test.properties (line 18)`
- `zheng-cms/zheng-cms-admin/src/main/resources/profiles/dev.properties (line 27)`
- `zheng-cms/zheng-cms-admin/src/main/resources/profiles/dev.properties (line 39)`
- `zheng-cms/zheng-cms-admin/src/main/resources/profiles/prod.properties (line 27)`
- `zheng-cms/zheng-cms-admin/src/main/resources/profiles/prod.properties (line 39)`
- `zheng-cms/zheng-cms-admin/src/main/resources/profiles/test.properties (line 27)`
- `zheng-cms/zheng-cms-admin/src/main/resources/profiles/test.properties (line 39)`
- `zheng-cms/zheng-cms-web/src/main/resources/profiles/test.properties (line 3)`
- `zheng-cms/zheng-cms-web/src/main/resources/profiles/dev.properties (line 3)`
- `zheng-cms/zheng-cms-web/src/main/resources/profiles/prod.properties (line 3)`
- `zheng-demo/zheng-demo-web/src/main/java/com/zheng/demo/web/controller/IndexController.java (line 45)`
- `zheng-demo/zheng-demo-web/src/main/resources/profiles/dev.properties (line 3)`
- `zheng-demo/zheng-demo-web/src/main/resources/profiles/dev.properties (line 9)`
- `zheng-demo/zheng-demo-web/src/main/resources/profiles/prod.properties (line 3)`
- `zheng-demo/zheng-demo-web/src/main/resources/profiles/prod.properties (line 9)`
- `zheng-demo/zheng-demo-web/src/main/resources/profiles/test.properties (line 3)`
- `zheng-demo/zheng-demo-web/src/main/resources/profiles/test.properties (line 9)`
- `zheng-message/zheng-message-sdk/src/main/java/com/zheng/message/sdk/MessageHelper.java (line 58)`
- `zheng-message/zheng-message-server/src/main/resources/profiles/dev.properties (line 3)`
- `zheng-message/zheng-message-server/src/main/resources/profiles/prod.properties (line 3)`
- `zheng-message/zheng-message-server/src/main/resources/profiles/test.properties (line 3)`
- `zheng-oss/zheng-oss-admin/src/main/resources/profiles/dev.properties (line 22)`
- `zheng-oss/zheng-oss-admin/src/main/resources/profiles/prod.properties (line 22)`
- `zheng-oss/zheng-oss-admin/src/main/resources/profiles/test.properties (line 22)`

</details>

<details id="Localhost_Usage">
<summary><b>Localhost Usage</b> — affected files</summary>

- `zheng-message/zheng-message-server/src/main/java/com/zheng/message/server/AckChatLauncher.java (line 16)`
- `zheng-message/zheng-message-server/src/main/java/com/zheng/message/server/BinaryEventLauncher.java (line 17)`
- `zheng-message/zheng-message-server/src/main/java/com/zheng/message/server/ChatLauncher.java (line 11)`
- `zheng-message/zheng-message-server/src/main/java/com/zheng/message/server/EventChatLauncher.java (line 14)`
- `zheng-message/zheng-message-server/src/main/java/com/zheng/message/server/NamespaceChatLauncher.java (line 11)`
- `zheng-message/zheng-message-server/src/main/java/com/zheng/message/server/SslChatLauncher.java (line 16)`
- `zheng-cms/zheng-cms-web/src/main/java/com/zheng/cms/web/rocketmq/Consumer.java (line 21)`
- `zheng-cms/zheng-cms-web/src/main/java/com/zheng/cms/web/rocketmq/Producer.java (line 14)`

</details>

## Upgrade Issues

| Issue Name | Criticality | Story Points | Occurrences |
|------------|-------------|--------------|-------------|
| Java Version Has Reached the End of Support | Mandatory | 8 | [42](#Java_Version_Has_Reached_the_End_of_Support) |

### Issue Details

<details id="Java_Version_Has_Reached_the_End_of_Support">
<summary><b>Java Version Has Reached the End of Support</b> — affected files</summary>

- `pom.xml (line 16)`
- `pom.xml (line 17)`
- `zheng-admin/pom.xml (line 16)`
- `zheng-admin/pom.xml (line 17)`
- `zheng-api/pom.xml (line 22)`
- `zheng-api/pom.xml (line 23)`
- `zheng-api/zheng-api-rpc-service/pom.xml (line 107)`
- `zheng-api/zheng-api-rpc-service/pom.xml (line 108)`
- `zheng-cms/pom.xml (line 16)`
- `zheng-cms/pom.xml (line 17)`
- `zheng-cms/zheng-cms-rpc-service/pom.xml (line 107)`
- `zheng-cms/zheng-cms-rpc-service/pom.xml (line 108)`
- `zheng-common/pom.xml (line 16)`
- `zheng-common/pom.xml (line 17)`
- `zheng-demo/pom.xml (line 16)`
- `zheng-demo/pom.xml (line 17)`
- `zheng-demo/zheng-demo-rpc-service/pom.xml (line 68)`
- `zheng-demo/zheng-demo-rpc-service/pom.xml (line 69)`
- `zheng-message/pom.xml (line 16)`
- `zheng-message/pom.xml (line 17)`
- `zheng-oss/pom.xml (line 16)`
- `zheng-oss/pom.xml (line 17)`
- `zheng-pay/pom.xml (line 16)`
- `zheng-pay/pom.xml (line 17)`
- `zheng-pay/zheng-pay-rpc-service/pom.xml (line 107)`
- `zheng-pay/zheng-pay-rpc-service/pom.xml (line 108)`
- `zheng-shop/pom.xml (line 16)`
- `zheng-shop/pom.xml (line 17)`
- `zheng-ucenter/pom.xml (line 16)`
- `zheng-ucenter/pom.xml (line 17)`
- `zheng-ucenter/zheng-ucenter-rpc-service/pom.xml (line 107)`
- `zheng-ucenter/zheng-ucenter-rpc-service/pom.xml (line 108)`
- `zheng-upms/pom.xml (line 16)`
- `zheng-upms/pom.xml (line 17)`
- `zheng-upms/zheng-upms-rpc-service/pom.xml (line 107)`
- `zheng-upms/zheng-upms-rpc-service/pom.xml (line 108)`
- `zheng-wechat/pom.xml (line 16)`
- `zheng-wechat/pom.xml (line 17)`
- `zheng-wechat/zheng-wechat-app/pom.xml (line 20)`
- `zheng-wechat/zheng-wechat-app/pom.xml (line 21)`
- `zheng-wechat/zheng-wechat-mp/pom.xml (line 20)`
- `zheng-wechat/zheng-wechat-mp/pom.xml (line 21)`

</details>

## Security Issues

> **Note:** These issues were generated by AI and may contain inaccuracies or incomplete information. Please review carefully.

| Issue Name | Criticality | Story Points | Files |
|------------|-------------|--------------|-------|
| CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection') | Mandatory | 13 | [3](#CWE-89_Improper_Neutralization_of_Special_Elements_used_in_an_SQL_Command_SQL_Injection) |
| CWE-502: Deserialization of Untrusted Data | Mandatory | 13 | [1](#CWE-502_Deserialization_of_Untrusted_Data) |
| CWE-434: Unrestricted Upload of File with Dangerous Type | Mandatory | 8 | [1](#CWE-434_Unrestricted_Upload_of_File_with_Dangerous_Type) |
| CVE-2026-49268: Apache Shiro: LDAP DN Injection in DefaultLdapRealm | Mandatory | 1 | [1](#CVE-2026-49268_Apache_Shiro_LDAP_DN_Injection_in_DefaultLdapRealm) |
| CVE-2025-70974: FASTJSON Includes Functionality from Untrusted Control Sphere  | Mandatory | 1 | [2](#CVE-2025-70974_FASTJSON_Includes_Functionality_from_Untrusted_Control_Sphere) |
| CVE-2025-52999: jackson-core can throw a StackoverflowError when processing deeply nested data | Mandatory | 1 | [1](#CVE-2025-52999_jackson-core_can_throw_a_StackoverflowError_when_processing_deeply_nested_data) |
| CVE-2025-48976: Apache Commons FileUpload, Apache Commons FileUpload: FileUpload DoS via part headers | Mandatory | 1 | [1](#CVE-2025-48976_Apache_Commons_FileUpload_Apache_Commons_FileUpload_FileUpload_DoS_via_part_headers) |
| CVE-2025-48734: Apache Commons Improper Access Control vulnerability | Mandatory | 1 | [1](#CVE-2025-48734_Apache_Commons_Improper_Access_Control_vulnerability) |
| CVE-2024-38819: Spring Framework Path Traversal vulnerability | Mandatory | 1 | [1](#CVE-2024-38819_Spring_Framework_Path_Traversal_vulnerability) |
| CVE-2023-22102: MySQL Connectors takeover vulnerability | Mandatory | 1 | [1](#CVE-2023-22102_MySQL_Connectors_takeover_vulnerability) |
| CVE-2023-34478: Path Traversal in Apache Shiro | Mandatory | 1 | [1](#CVE-2023-34478_Path_Traversal_in_Apache_Shiro) |
| CVE-2023-24998: Apache Commons FileUpload denial of service vulnerability | Mandatory | 1 | [1](#CVE-2023-24998_Apache_Commons_FileUpload_denial_of_service_vulnerability) |
| CVE-2022-40664: Apache Shiro Authentication Bypass vulnerability | Mandatory | 1 | [1](#CVE-2022-40664_Apache_Shiro_Authentication_Bypass_vulnerability) |
| CVE-2022-42003: Uncontrolled Resource Consumption in Jackson-databind | Mandatory | 1 | [1](#CVE-2022-42003_Uncontrolled_Resource_Consumption_in_Jackson-databind) |
| CVE-2022-42004: Uncontrolled Resource Consumption in FasterXML jackson-databind | Mandatory | 1 | [1](#CVE-2022-42004_Uncontrolled_Resource_Consumption_in_FasterXML_jackson-databind) |
| CVE-2020-10650: jackson-databind vulnerable to unsafe deserialization | Mandatory | 1 | [1](#CVE-2020-10650_jackson-databind_vulnerable_to_unsafe_deserialization) |
| CVE-2022-32532: Improper Authorization in Apache Shiro | Mandatory | 1 | [1](#CVE-2022-32532_Improper_Authorization_in_Apache_Shiro) |
| CVE-2022-25845: Unsafe deserialization in com.alibaba:fastjson | Mandatory | 1 | [2](#CVE-2022-25845_Unsafe_deserialization_in_com_alibaba_fastjson) |
| CVE-2018-3258: Improper Privilege Management in MySQL Connectors Java | Mandatory | 1 | [1](#CVE-2018-3258_Improper_Privilege_Management_in_MySQL_Connectors_Java) |
| CVE-2017-3523: Improper Access Control in MySQL Connectors Java | Mandatory | 1 | [1](#CVE-2017-3523_Improper_Access_Control_in_MySQL_Connectors_Java) |
| CVE-2022-28111: MyBatis PageHelper vulnerable to time-blind SQL injection via orderBy parameter | Mandatory | 1 | [1](#CVE-2022-28111_MyBatis_PageHelper_vulnerable_to_time-blind_SQL_injection_via_orderBy_parameter) |
| CVE-2022-22965: Remote Code Execution in Spring Framework | Mandatory | 1 | [1](#CVE-2022-22965_Remote_Code_Execution_in_Spring_Framework) |
| CVE-2020-36518: Deeply nested json in jackson-databind | Mandatory | 1 | [1](#CVE-2020-36518_Deeply_nested_json_in_jackson-databind) |
| CVE-2020-17523: Authentication bypass in Apache Shiro | Mandatory | 1 | [2](#CVE-2020-17523_Authentication_bypass_in_Apache_Shiro) |
| CVE-2020-13936: Sandbox Bypass in Apache Velocity Engine | Mandatory | 1 | [1](#CVE-2020-13936_Sandbox_Bypass_in_Apache_Velocity_Engine) |
| CVE-2020-36189: Unsafe Deserialization in jackson-databind | Mandatory | 1 | [1](#CVE-2020-36189_Unsafe_Deserialization_in_jackson-databind) |
| CVE-2020-36187: Unsafe Deserialization in jackson-databind | Mandatory | 1 | [1](#CVE-2020-36187_Unsafe_Deserialization_in_jackson-databind) |
| CVE-2020-36188: Unsafe Deserialization in jackson-databind | Mandatory | 1 | [1](#CVE-2020-36188_Unsafe_Deserialization_in_jackson-databind) |
| CVE-2020-36183: Unsafe Deserialization in jackson-databind | Mandatory | 1 | [1](#CVE-2020-36183_Unsafe_Deserialization_in_jackson-databind) |
| CVE-2020-36184: Unsafe Deserialization in jackson-databind | Mandatory | 1 | [1](#CVE-2020-36184_Unsafe_Deserialization_in_jackson-databind) |
| CVE-2020-36180: Unsafe Deserialization in jackson-databind | Mandatory | 1 | [1](#CVE-2020-36180_Unsafe_Deserialization_in_jackson-databind) |
| CVE-2020-36181: Unsafe Deserialization in jackson-databind | Mandatory | 1 | [1](#CVE-2020-36181_Unsafe_Deserialization_in_jackson-databind) |
| CVE-2020-36185: Unsafe Deserialization in jackson-databind | Mandatory | 1 | [1](#CVE-2020-36185_Unsafe_Deserialization_in_jackson-databind) |
| CVE-2020-36179: Unsafe Deserialization in jackson-databind | Mandatory | 1 | [1](#CVE-2020-36179_Unsafe_Deserialization_in_jackson-databind) |
| CVE-2020-36182: Unsafe Deserialization in jackson-databind | Mandatory | 1 | [1](#CVE-2020-36182_Unsafe_Deserialization_in_jackson-databind) |
| CVE-2020-24750: Unsafe Deserialization in jackson-databind | Mandatory | 1 | [1](#CVE-2020-24750_Unsafe_Deserialization_in_jackson-databind) |
| CVE-2020-35728: Serialization gadget exploit in jackson-databind | Mandatory | 1 | [1](#CVE-2020-35728_Serialization_gadget_exploit_in_jackson-databind) |
| CVE-2020-35491: Serialization gadgets exploit in jackson-databind | Mandatory | 1 | [1](#CVE-2020-35491_Serialization_gadgets_exploit_in_jackson-databind) |
| CVE-2020-35490: Serialization gadgets exploit in jackson-databind | Mandatory | 1 | [1](#CVE-2020-35490_Serialization_gadgets_exploit_in_jackson-databind) |
| CVE-2020-24616: Code Injection in jackson-databind | Mandatory | 1 | [1](#CVE-2020-24616_Code_Injection_in_jackson-databind) |
| CVE-2020-36186: Unsafe Deserialization in jackson-databind | Mandatory | 1 | [1](#CVE-2020-36186_Unsafe_Deserialization_in_jackson-databind) |
| CVE-2021-41303: Apache Shiro vulnerable to a specially crafted HTTP request causing an authentication bypass | Mandatory | 1 | [1](#CVE-2021-41303_Apache_Shiro_vulnerable_to_a_specially_crafted_HTTP_request_causing_an_authentication_bypass) |
| CVE-2021-36090: Improper Handling of Length Parameter Inconsistency in Compress | Mandatory | 1 | [1](#CVE-2021-36090_Improper_Handling_of_Length_Parameter_Inconsistency_in_Compress) |
| CVE-2021-35517: Improper Handling of Length Parameter Inconsistency in Compress | Mandatory | 1 | [1](#CVE-2021-35517_Improper_Handling_of_Length_Parameter_Inconsistency_in_Compress) |
| CVE-2021-35516: Improper Handling of Length Parameter Inconsistency in Compress | Mandatory | 1 | [1](#CVE-2021-35516_Improper_Handling_of_Length_Parameter_Inconsistency_in_Compress) |
| CVE-2021-35515: Excessive Iteration in Compress | Mandatory | 1 | [1](#CVE-2021-35515_Excessive_Iteration_in_Compress) |
| CVE-2020-13933: Authentication bypass in Apache Shiro | Mandatory | 1 | [1](#CVE-2020-13933_Authentication_bypass_in_Apache_Shiro) |
| CVE-2020-1957: Improper Authentication in Apache Shiro | Mandatory | 1 | [1](#CVE-2020-1957_Improper_Authentication_in_Apache_Shiro) |
| CVE-2020-11989: Improper Authentication in Apache Shiro | Mandatory | 1 | [1](#CVE-2020-11989_Improper_Authentication_in_Apache_Shiro) |
| CVE-2020-26945: "Deserialization errors in MyBatis" | Mandatory | 1 | [1](#CVE-2020-26945_Deserialization_errors_in_MyBatis) |
| CVE-2020-17510: Authentication bypass in Apache Shiro | Mandatory | 1 | [1](#CVE-2020-17510_Authentication_bypass_in_Apache_Shiro) |
| CVE-2020-25649: XML External Entity (XXE) Injection in Jackson Databind | Mandatory | 1 | [1](#CVE-2020-25649_XML_External_Entity_XXE_Injection_in_Jackson_Databind) |
| CVE-2021-20190: Deserialization of untrusted data in jackson-databind | Mandatory | 1 | [1](#CVE-2021-20190_Deserialization_of_untrusted_data_in_jackson-databind) |
| CVE-2020-14061: Deserialization of untrusted data in Jackson Databind | Mandatory | 1 | [1](#CVE-2020-14061_Deserialization_of_untrusted_data_in_Jackson_Databind) |
| CVE-2020-14062: Deserialization of untrusted data in Jackson Databind | Mandatory | 1 | [1](#CVE-2020-14062_Deserialization_of_untrusted_data_in_Jackson_Databind) |
| CVE-2020-14060: Deserialization of untrusted data in Jackson Databind | Mandatory | 1 | [1](#CVE-2020-14060_Deserialization_of_untrusted_data_in_Jackson_Databind) |
| CVE-2020-14195: Deserialization of untrusted data in Jackson Databind | Mandatory | 1 | [1](#CVE-2020-14195_Deserialization_of_untrusted_data_in_Jackson_Databind) |
| CVE-2019-10086: Insecure Deserialization in Apache Commons Beanutils | Mandatory | 1 | [1](#CVE-2019-10086_Insecure_Deserialization_in_Apache_Commons_Beanutils) |
| CVE-2017-7536: Privilege Escalation in Hibernate Validator | Mandatory | 1 | [1](#CVE-2017-7536_Privilege_Escalation_in_Hibernate_Validator) |
| CVE-2019-17267: Improper Input Validation in jackson-databind | Mandatory | 1 | [1](#CVE-2019-17267_Improper_Input_Validation_in_jackson-databind) |
| CVE-2014-0114: Arbitrary code execution in Apache Commons BeanUtils | Mandatory | 1 | [1](#CVE-2014-0114_Arbitrary_code_execution_in_Apache_Commons_BeanUtils) |
| CVE-2020-11112: jackson-databind mishandles the interaction between serialization gadgets and typing | Mandatory | 1 | [1](#CVE-2020-11112_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing) |
| CVE-2020-9547: jackson-databind mishandles the interaction between serialization gadgets and typing | Mandatory | 1 | [1](#CVE-2020-9547_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing) |
| CVE-2019-14893: Polymorphic deserialization of malicious object in jackson-databind | Mandatory | 1 | [1](#CVE-2019-14893_Polymorphic_deserialization_of_malicious_object_in_jackson-databind) |
| CVE-2020-10673: jackson-databind mishandles the interaction between serialization gadgets and typing | Mandatory | 1 | [1](#CVE-2020-10673_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing) |
| CVE-2020-9548: jackson-databind mishandles the interaction between serialization gadgets and typing | Mandatory | 1 | [1](#CVE-2020-9548_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing) |
| CVE-2019-14892: Polymorphic deserialization of malicious object in jackson-databind | Mandatory | 1 | [1](#CVE-2019-14892_Polymorphic_deserialization_of_malicious_object_in_jackson-databind) |
| CVE-2020-10968: jackson-databind mishandles the interaction between serialization gadgets and typing | Mandatory | 1 | [1](#CVE-2020-10968_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing) |
| CVE-2020-11111: jackson-databind mishandles the interaction between serialization gadgets and typing | Mandatory | 1 | [1](#CVE-2020-11111_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing) |
| CVE-2020-11113: jackson-databind mishandles the interaction between serialization gadgets and typing | Mandatory | 1 | [1](#CVE-2020-11113_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing) |
| CVE-2020-11619: jackson-databind mishandles the interaction between serialization gadgets and typing | Mandatory | 1 | [1](#CVE-2020-11619_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing) |
| CVE-2020-10969: jackson-databind mishandles the interaction between serialization gadgets and typing | Mandatory | 1 | [1](#CVE-2020-10969_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing) |
| CVE-2020-9546: jackson-databind mishandles the interaction between serialization gadgets and typing | Mandatory | 1 | [1](#CVE-2020-9546_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing) |
| CVE-2020-11620: jackson-databind mishandles the interaction between serialization gadgets and typing | Mandatory | 1 | [1](#CVE-2020-11620_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing) |
| CVE-2020-10672: jackson-databind mishandles the interaction between serialization gadgets and typing | Mandatory | 1 | [1](#CVE-2020-10672_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing) |
| CVE-2020-8840: Deserialization of Untrusted Data in jackson-databind | Mandatory | 1 | [1](#CVE-2020-8840_Deserialization_of_Untrusted_Data_in_jackson-databind) |
| CVE-2019-20330: Deserialization of Untrusted Data in jackson-databind | Mandatory | 1 | [1](#CVE-2019-20330_Deserialization_of_Untrusted_Data_in_jackson-databind) |
| CVE-2019-12422: Improper input validation in Apache Shiro | Mandatory | 1 | [1](#CVE-2019-12422_Improper_input_validation_in_Apache_Shiro) |
| CVE-2019-17531: jackson-databind polymorphic typing issue | Mandatory | 1 | [1](#CVE-2019-17531_jackson-databind_polymorphic_typing_issue) |
| CVE-2019-16943: jackson-databind polymorphic typing issue | Mandatory | 1 | [1](#CVE-2019-16943_jackson-databind_polymorphic_typing_issue) |
| CVE-2019-16942: Polymorphic Typing in FasterXML jackson-databind | Mandatory | 1 | [1](#CVE-2019-16942_Polymorphic_Typing_in_FasterXML_jackson-databind) |
| CVE-2019-12402: Denial of Service in Apache Commons Compress | Mandatory | 1 | [1](#CVE-2019-12402_Denial_of_Service_in_Apache_Commons_Compress) |
| CVE-2019-16335: Polymorphic Typing issue in FasterXML jackson-databind | Mandatory | 1 | [1](#CVE-2019-16335_Polymorphic_Typing_issue_in_FasterXML_jackson-databind) |
| CVE-2019-14540: Polymorphic Typing issue in FasterXML jackson-databind | Mandatory | 1 | [1](#CVE-2019-14540_Polymorphic_Typing_issue_in_FasterXML_jackson-databind) |
| CVE-2026-22732: Spring Security HTTP Headers Are not Written Under Some Conditions | Mandatory | 1 | [1](#CVE-2026-22732_Spring_Security_HTTP_Headers_Are_not_Written_Under_Some_Conditions) |
| CVE-2024-38821: Spring Security vulnerable to Authorization Bypass of Static Resources in WebFlux Applications | Mandatory | 1 | [1](#CVE-2024-38821_Spring_Security_vulnerable_to_Authorization_Bypass_of_Static_Resources_in_WebFlux_Applications) |
| CVE-2022-22978: Authorization bypass in Spring Security | Mandatory | 1 | [1](#CVE-2022-22978_Authorization_bypass_in_Spring_Security) |
| CVE-2021-22112: Privilege escalation in spring security | Mandatory | 1 | [1](#CVE-2021-22112_Privilege_escalation_in_spring_security) |
| CWE-1057: Data Access Operations Outside of Expected Data Manager Component | Potential | 5 | [2](#CWE-1057_Data_Access_Operations_Outside_of_Expected_Data_Manager_Component) |
| CWE-321: Use of Hard-coded Cryptographic Key | Potential | 5 | [1](#CWE-321_Use_of_Hard-coded_Cryptographic_Key) |
| CWE-772: Missing Release of Resource after Effective Lifetime | Potential | 3 | [1](#CWE-772_Missing_Release_of_Resource_after_Effective_Lifetime) |
| CWE-775: Missing Release of File Descriptor or Handle after Effective Lifetime | Potential | 3 | [1](#CWE-775_Missing_Release_of_File_Descriptor_or_Handle_after_Effective_Lifetime) |
| CWE-778: Insufficient Logging | Potential | 3 | [1](#CWE-778_Insufficient_Logging) |
| CWE-22: Improper Limitation of a Pathname to a Restricted Directory ('Path Traversal') | Optional | 8 | [1](#CWE-22_Improper_Limitation_of_a_Pathname_to_a_Restricted_Directory_Path_Traversal) |
| CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting') | Optional | 8 | [2](#CWE-79_Improper_Neutralization_of_Input_During_Web_Page_Generation_Cross-site_Scripting) |
| CWE-259: Use of Hard-coded Password | Optional | 5 | [2](#CWE-259_Use_of_Hard-coded_Password) |
| CWE-798: Use of Hard-coded Credentials | Optional | 5 | [2](#CWE-798_Use_of_Hard-coded_Credentials) |
| CWE-23: Relative Path Traversal | Optional | 5 | [1](#CWE-23_Relative_Path_Traversal) |
| CWE-477: Use of Obsolete Function | Optional | 1 | [2](#CWE-477_Use_of_Obsolete_Function) |

### Security Issue Details

<details id="CWE-89_Improper_Neutralization_of_Special_Elements_used_in_an_SQL_Command_SQL_Injection">
<summary><b>CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')</b> — affected files</summary>

- `zheng-cms/zheng-cms-web/src/main/java/com/zheng/cms/web/controller/BlogController.java`
- `zheng-cms/zheng-cms-web/src/main/java/com/zheng/cms/web/controller/SearchController.java`
- `zheng-cms/zheng-cms-web/src/main/java/com/zheng/cms/web/controller/QaController.java`

</details>

<details id="CWE-502_Deserialization_of_Untrusted_Data">
<summary><b>CWE-502: Deserialization of Untrusted Data</b> — affected files</summary>

- `zheng-common/pom.xml`

</details>

<details id="CWE-434_Unrestricted_Upload_of_File_with_Dangerous_Type">
<summary><b>CWE-434: Unrestricted Upload of File with Dangerous Type</b> — affected files</summary>

- `zheng-oss/zheng-oss-web/src/main/java/com/zheng/oss/web/service/AliyunOssService.java`

</details>

<details id="CVE-2026-49268_Apache_Shiro_LDAP_DN_Injection_in_DefaultLdapRealm">
<summary><b>CVE-2026-49268: Apache Shiro: LDAP DN Injection in DefaultLdapRealm</b> — affected files</summary>

- `zheng-common/pom.xml:85`

</details>

<details id="CVE-2025-70974_FASTJSON_Includes_Functionality_from_Untrusted_Control_Sphere">
<summary><b>CVE-2025-70974: FASTJSON Includes Functionality from Untrusted Control Sphere </b> — affected files</summary>

- `zheng-common/pom.xml:284`
- `zheng-message/zheng-message-sdk/pom.xml:27`

</details>

<details id="CVE-2025-52999_jackson-core_can_throw_a_StackoverflowError_when_processing_deeply_nested_data">
<summary><b>CVE-2025-52999: jackson-core can throw a StackoverflowError when processing deeply nested data</b> — affected files</summary>

- `zheng-common/pom.xml:289`

</details>

<details id="CVE-2025-48976_Apache_Commons_FileUpload_Apache_Commons_FileUpload_FileUpload_DoS_via_part_headers">
<summary><b>CVE-2025-48976: Apache Commons FileUpload, Apache Commons FileUpload: FileUpload DoS via part headers</b> — affected files</summary>

- `zheng-common/pom.xml:201`

</details>

<details id="CVE-2025-48734_Apache_Commons_Improper_Access_Control_vulnerability">
<summary><b>CVE-2025-48734: Apache Commons Improper Access Control vulnerability</b> — affected files</summary>

- `zheng-common/pom.xml:218`

</details>

<details id="CVE-2024-38819_Spring_Framework_Path_Traversal_vulnerability">
<summary><b>CVE-2024-38819: Spring Framework Path Traversal vulnerability</b> — affected files</summary>

- `zheng-common/pom.xml:47`

</details>

<details id="CVE-2023-22102_MySQL_Connectors_takeover_vulnerability">
<summary><b>CVE-2023-22102: MySQL Connectors takeover vulnerability</b> — affected files</summary>

- `zheng-common/pom.xml:167`

</details>

<details id="CVE-2023-34478_Path_Traversal_in_Apache_Shiro">
<summary><b>CVE-2023-34478: Path Traversal in Apache Shiro</b> — affected files</summary>

- `zheng-common/pom.xml:90`

</details>

<details id="CVE-2023-24998_Apache_Commons_FileUpload_denial_of_service_vulnerability">
<summary><b>CVE-2023-24998: Apache Commons FileUpload denial of service vulnerability</b> — affected files</summary>

- `zheng-common/pom.xml:201`

</details>

<details id="CVE-2022-40664_Apache_Shiro_Authentication_Bypass_vulnerability">
<summary><b>CVE-2022-40664: Apache Shiro Authentication Bypass vulnerability</b> — affected files</summary>

- `zheng-common/pom.xml:85`

</details>

<details id="CVE-2022-42003_Uncontrolled_Resource_Consumption_in_Jackson-databind">
<summary><b>CVE-2022-42003: Uncontrolled Resource Consumption in Jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2022-42004_Uncontrolled_Resource_Consumption_in_FasterXML_jackson-databind">
<summary><b>CVE-2022-42004: Uncontrolled Resource Consumption in FasterXML jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-10650_jackson-databind_vulnerable_to_unsafe_deserialization">
<summary><b>CVE-2020-10650: jackson-databind vulnerable to unsafe deserialization</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2022-32532_Improper_Authorization_in_Apache_Shiro">
<summary><b>CVE-2022-32532: Improper Authorization in Apache Shiro</b> — affected files</summary>

- `zheng-common/pom.xml:85`

</details>

<details id="CVE-2022-25845_Unsafe_deserialization_in_com_alibaba_fastjson">
<summary><b>CVE-2022-25845: Unsafe deserialization in com.alibaba:fastjson</b> — affected files</summary>

- `zheng-common/pom.xml:284`
- `zheng-message/zheng-message-sdk/pom.xml:27`

</details>

<details id="CVE-2018-3258_Improper_Privilege_Management_in_MySQL_Connectors_Java">
<summary><b>CVE-2018-3258: Improper Privilege Management in MySQL Connectors Java</b> — affected files</summary>

- `zheng-common/pom.xml:167`

</details>

<details id="CVE-2017-3523_Improper_Access_Control_in_MySQL_Connectors_Java">
<summary><b>CVE-2017-3523: Improper Access Control in MySQL Connectors Java</b> — affected files</summary>

- `zheng-common/pom.xml:167`

</details>

<details id="CVE-2022-28111_MyBatis_PageHelper_vulnerable_to_time-blind_SQL_injection_via_orderBy_parameter">
<summary><b>CVE-2022-28111: MyBatis PageHelper vulnerable to time-blind SQL injection via orderBy parameter</b> — affected files</summary>

- `zheng-common/pom.xml:116`

</details>

<details id="CVE-2022-22965_Remote_Code_Execution_in_Spring_Framework">
<summary><b>CVE-2022-22965: Remote Code Execution in Spring Framework</b> — affected files</summary>

- `zheng-common/pom.xml:47`

</details>

<details id="CVE-2020-36518_Deeply_nested_json_in_jackson-databind">
<summary><b>CVE-2020-36518: Deeply nested json in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-17523_Authentication_bypass_in_Apache_Shiro">
<summary><b>CVE-2020-17523: Authentication bypass in Apache Shiro</b> — affected files</summary>

- `zheng-common/pom.xml:90`
- `zheng-common/pom.xml:100`

</details>

<details id="CVE-2020-13936_Sandbox_Bypass_in_Apache_Velocity_Engine">
<summary><b>CVE-2020-13936: Sandbox Bypass in Apache Velocity Engine</b> — affected files</summary>

- `zheng-common/pom.xml:144`

</details>

<details id="CVE-2020-36189_Unsafe_Deserialization_in_jackson-databind">
<summary><b>CVE-2020-36189: Unsafe Deserialization in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-36187_Unsafe_Deserialization_in_jackson-databind">
<summary><b>CVE-2020-36187: Unsafe Deserialization in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-36188_Unsafe_Deserialization_in_jackson-databind">
<summary><b>CVE-2020-36188: Unsafe Deserialization in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-36183_Unsafe_Deserialization_in_jackson-databind">
<summary><b>CVE-2020-36183: Unsafe Deserialization in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-36184_Unsafe_Deserialization_in_jackson-databind">
<summary><b>CVE-2020-36184: Unsafe Deserialization in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-36180_Unsafe_Deserialization_in_jackson-databind">
<summary><b>CVE-2020-36180: Unsafe Deserialization in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-36181_Unsafe_Deserialization_in_jackson-databind">
<summary><b>CVE-2020-36181: Unsafe Deserialization in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-36185_Unsafe_Deserialization_in_jackson-databind">
<summary><b>CVE-2020-36185: Unsafe Deserialization in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-36179_Unsafe_Deserialization_in_jackson-databind">
<summary><b>CVE-2020-36179: Unsafe Deserialization in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-36182_Unsafe_Deserialization_in_jackson-databind">
<summary><b>CVE-2020-36182: Unsafe Deserialization in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-24750_Unsafe_Deserialization_in_jackson-databind">
<summary><b>CVE-2020-24750: Unsafe Deserialization in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-35728_Serialization_gadget_exploit_in_jackson-databind">
<summary><b>CVE-2020-35728: Serialization gadget exploit in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-35491_Serialization_gadgets_exploit_in_jackson-databind">
<summary><b>CVE-2020-35491: Serialization gadgets exploit in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-35490_Serialization_gadgets_exploit_in_jackson-databind">
<summary><b>CVE-2020-35490: Serialization gadgets exploit in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-24616_Code_Injection_in_jackson-databind">
<summary><b>CVE-2020-24616: Code Injection in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-36186_Unsafe_Deserialization_in_jackson-databind">
<summary><b>CVE-2020-36186: Unsafe Deserialization in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2021-41303_Apache_Shiro_vulnerable_to_a_specially_crafted_HTTP_request_causing_an_authentication_bypass">
<summary><b>CVE-2021-41303: Apache Shiro vulnerable to a specially crafted HTTP request causing an authentication bypass</b> — affected files</summary>

- `zheng-common/pom.xml:85`

</details>

<details id="CVE-2021-36090_Improper_Handling_of_Length_Parameter_Inconsistency_in_Compress">
<summary><b>CVE-2021-36090: Improper Handling of Length Parameter Inconsistency in Compress</b> — affected files</summary>

- `zheng-common/pom.xml:233`

</details>

<details id="CVE-2021-35517_Improper_Handling_of_Length_Parameter_Inconsistency_in_Compress">
<summary><b>CVE-2021-35517: Improper Handling of Length Parameter Inconsistency in Compress</b> — affected files</summary>

- `zheng-common/pom.xml:233`

</details>

<details id="CVE-2021-35516_Improper_Handling_of_Length_Parameter_Inconsistency_in_Compress">
<summary><b>CVE-2021-35516: Improper Handling of Length Parameter Inconsistency in Compress</b> — affected files</summary>

- `zheng-common/pom.xml:233`

</details>

<details id="CVE-2021-35515_Excessive_Iteration_in_Compress">
<summary><b>CVE-2021-35515: Excessive Iteration in Compress</b> — affected files</summary>

- `zheng-common/pom.xml:233`

</details>

<details id="CVE-2020-13933_Authentication_bypass_in_Apache_Shiro">
<summary><b>CVE-2020-13933: Authentication bypass in Apache Shiro</b> — affected files</summary>

- `zheng-common/pom.xml:85`

</details>

<details id="CVE-2020-1957_Improper_Authentication_in_Apache_Shiro">
<summary><b>CVE-2020-1957: Improper Authentication in Apache Shiro</b> — affected files</summary>

- `zheng-common/pom.xml:85`

</details>

<details id="CVE-2020-11989_Improper_Authentication_in_Apache_Shiro">
<summary><b>CVE-2020-11989: Improper Authentication in Apache Shiro</b> — affected files</summary>

- `zheng-common/pom.xml:85`

</details>

<details id="CVE-2020-26945_Deserialization_errors_in_MyBatis">
<summary><b>CVE-2020-26945: &quot;Deserialization errors in MyBatis&quot;</b> — affected files</summary>

- `zheng-common/pom.xml:106`

</details>

<details id="CVE-2020-17510_Authentication_bypass_in_Apache_Shiro">
<summary><b>CVE-2020-17510: Authentication bypass in Apache Shiro</b> — affected files</summary>

- `zheng-common/pom.xml:100`

</details>

<details id="CVE-2020-25649_XML_External_Entity_XXE_Injection_in_Jackson_Databind">
<summary><b>CVE-2020-25649: XML External Entity (XXE) Injection in Jackson Databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2021-20190_Deserialization_of_untrusted_data_in_jackson-databind">
<summary><b>CVE-2021-20190: Deserialization of untrusted data in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-14061_Deserialization_of_untrusted_data_in_Jackson_Databind">
<summary><b>CVE-2020-14061: Deserialization of untrusted data in Jackson Databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-14062_Deserialization_of_untrusted_data_in_Jackson_Databind">
<summary><b>CVE-2020-14062: Deserialization of untrusted data in Jackson Databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-14060_Deserialization_of_untrusted_data_in_Jackson_Databind">
<summary><b>CVE-2020-14060: Deserialization of untrusted data in Jackson Databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-14195_Deserialization_of_untrusted_data_in_Jackson_Databind">
<summary><b>CVE-2020-14195: Deserialization of untrusted data in Jackson Databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2019-10086_Insecure_Deserialization_in_Apache_Commons_Beanutils">
<summary><b>CVE-2019-10086: Insecure Deserialization in Apache Commons Beanutils</b> — affected files</summary>

- `zheng-common/pom.xml:218`

</details>

<details id="CVE-2017-7536_Privilege_Escalation_in_Hibernate_Validator">
<summary><b>CVE-2017-7536: Privilege Escalation in Hibernate Validator</b> — affected files</summary>

- `zheng-common/pom.xml:254`

</details>

<details id="CVE-2019-17267_Improper_Input_Validation_in_jackson-databind">
<summary><b>CVE-2019-17267: Improper Input Validation in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2014-0114_Arbitrary_code_execution_in_Apache_Commons_BeanUtils">
<summary><b>CVE-2014-0114: Arbitrary code execution in Apache Commons BeanUtils</b> — affected files</summary>

- `zheng-common/pom.xml:218`

</details>

<details id="CVE-2020-11112_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing">
<summary><b>CVE-2020-11112: jackson-databind mishandles the interaction between serialization gadgets and typing</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-9547_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing">
<summary><b>CVE-2020-9547: jackson-databind mishandles the interaction between serialization gadgets and typing</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2019-14893_Polymorphic_deserialization_of_malicious_object_in_jackson-databind">
<summary><b>CVE-2019-14893: Polymorphic deserialization of malicious object in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-10673_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing">
<summary><b>CVE-2020-10673: jackson-databind mishandles the interaction between serialization gadgets and typing</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-9548_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing">
<summary><b>CVE-2020-9548: jackson-databind mishandles the interaction between serialization gadgets and typing</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2019-14892_Polymorphic_deserialization_of_malicious_object_in_jackson-databind">
<summary><b>CVE-2019-14892: Polymorphic deserialization of malicious object in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-10968_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing">
<summary><b>CVE-2020-10968: jackson-databind mishandles the interaction between serialization gadgets and typing</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-11111_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing">
<summary><b>CVE-2020-11111: jackson-databind mishandles the interaction between serialization gadgets and typing</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-11113_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing">
<summary><b>CVE-2020-11113: jackson-databind mishandles the interaction between serialization gadgets and typing</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-11619_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing">
<summary><b>CVE-2020-11619: jackson-databind mishandles the interaction between serialization gadgets and typing</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-10969_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing">
<summary><b>CVE-2020-10969: jackson-databind mishandles the interaction between serialization gadgets and typing</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-9546_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing">
<summary><b>CVE-2020-9546: jackson-databind mishandles the interaction between serialization gadgets and typing</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-11620_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing">
<summary><b>CVE-2020-11620: jackson-databind mishandles the interaction between serialization gadgets and typing</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-10672_jackson-databind_mishandles_the_interaction_between_serialization_gadgets_and_typing">
<summary><b>CVE-2020-10672: jackson-databind mishandles the interaction between serialization gadgets and typing</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2020-8840_Deserialization_of_Untrusted_Data_in_jackson-databind">
<summary><b>CVE-2020-8840: Deserialization of Untrusted Data in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2019-20330_Deserialization_of_Untrusted_Data_in_jackson-databind">
<summary><b>CVE-2019-20330: Deserialization of Untrusted Data in jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2019-12422_Improper_input_validation_in_Apache_Shiro">
<summary><b>CVE-2019-12422: Improper input validation in Apache Shiro</b> — affected files</summary>

- `zheng-common/pom.xml:85`

</details>

<details id="CVE-2019-17531_jackson-databind_polymorphic_typing_issue">
<summary><b>CVE-2019-17531: jackson-databind polymorphic typing issue</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2019-16943_jackson-databind_polymorphic_typing_issue">
<summary><b>CVE-2019-16943: jackson-databind polymorphic typing issue</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2019-16942_Polymorphic_Typing_in_FasterXML_jackson-databind">
<summary><b>CVE-2019-16942: Polymorphic Typing in FasterXML jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2019-12402_Denial_of_Service_in_Apache_Commons_Compress">
<summary><b>CVE-2019-12402: Denial of Service in Apache Commons Compress</b> — affected files</summary>

- `zheng-common/pom.xml:233`

</details>

<details id="CVE-2019-16335_Polymorphic_Typing_issue_in_FasterXML_jackson-databind">
<summary><b>CVE-2019-16335: Polymorphic Typing issue in FasterXML jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2019-14540_Polymorphic_Typing_issue_in_FasterXML_jackson-databind">
<summary><b>CVE-2019-14540: Polymorphic Typing issue in FasterXML jackson-databind</b> — affected files</summary>

- `zheng-common/pom.xml:294`

</details>

<details id="CVE-2026-22732_Spring_Security_HTTP_Headers_Are_not_Written_Under_Some_Conditions">
<summary><b>CVE-2026-22732: Spring Security HTTP Headers Are not Written Under Some Conditions</b> — affected files</summary>

- `zheng-common/pom.xml:68`

</details>

<details id="CVE-2024-38821_Spring_Security_vulnerable_to_Authorization_Bypass_of_Static_Resources_in_WebFlux_Applications">
<summary><b>CVE-2024-38821: Spring Security vulnerable to Authorization Bypass of Static Resources in WebFlux Applications</b> — affected files</summary>

- `zheng-common/pom.xml:68`

</details>

<details id="CVE-2022-22978_Authorization_bypass_in_Spring_Security">
<summary><b>CVE-2022-22978: Authorization bypass in Spring Security</b> — affected files</summary>

- `zheng-common/pom.xml:68`

</details>

<details id="CVE-2021-22112_Privilege_escalation_in_spring_security">
<summary><b>CVE-2021-22112: Privilege escalation in spring security</b> — affected files</summary>

- `zheng-common/pom.xml:68`

</details>

<details id="CWE-1057_Data_Access_Operations_Outside_of_Expected_Data_Manager_Component">
<summary><b>CWE-1057: Data Access Operations Outside of Expected Data Manager Component</b> — affected files</summary>

- `zheng-common/src/main/java/com/zheng/common/util/JdbcUtil.java`
- `zheng-common/src/main/java/com/zheng/common/util/MybatisGeneratorUtil.java`

</details>

<details id="CWE-321_Use_of_Hard-coded_Cryptographic_Key">
<summary><b>CWE-321: Use of Hard-coded Cryptographic Key</b> — affected files</summary>

- `zheng-common/src/main/java/com/zheng/common/util/AESUtil.java`

</details>

<details id="CWE-772_Missing_Release_of_Resource_after_Effective_Lifetime">
<summary><b>CWE-772: Missing Release of Resource after Effective Lifetime</b> — affected files</summary>

- `zheng-common/src/main/java/com/zheng/common/util/MybatisGeneratorUtil.java`

</details>

<details id="CWE-775_Missing_Release_of_File_Descriptor_or_Handle_after_Effective_Lifetime">
<summary><b>CWE-775: Missing Release of File Descriptor or Handle after Effective Lifetime</b> — affected files</summary>

- `zheng-common/src/main/java/com/zheng/common/util/VelocityUtil.java`

</details>

<details id="CWE-778_Insufficient_Logging">
<summary><b>CWE-778: Insufficient Logging</b> — affected files</summary>

- `zheng-upms/zheng-upms-server/src/main/java/com/zheng/upms/server/controller/SSOController.java`

</details>

<details id="CWE-22_Improper_Limitation_of_a_Pathname_to_a_Restricted_Directory_Path_Traversal">
<summary><b>CWE-22: Improper Limitation of a Pathname to a Restricted Directory ('Path Traversal')</b> — affected files</summary>

- `zheng-common/src/main/java/com/zheng/common/util/JarUtil.java`

</details>

<details id="CWE-79_Improper_Neutralization_of_Input_During_Web_Page_Generation_Cross-site_Scripting">
<summary><b>CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')</b> — affected files</summary>

- `zheng-ui/zheng-cms-web/blog/details/index.html`
- `zheng-api/zheng-api-server/src/main/webapp/WEB-INF/jsp/403.jsp`

</details>

<details id="CWE-259_Use_of_Hard-coded_Password">
<summary><b>CWE-259: Use of Hard-coded Password</b> — affected files</summary>

- `zheng-upms/zheng-upms-rpc-service/src/main/resources/profiles/dev.properties`
- `zheng-common/src/main/java/com/zheng/common/util/AESUtil.java`

</details>

<details id="CWE-798_Use_of_Hard-coded_Credentials">
<summary><b>CWE-798: Use of Hard-coded Credentials</b> — affected files</summary>

- `zheng-common/src/main/java/com/zheng/common/util/AESUtil.java`
- `zheng-upms/zheng-upms-rpc-service/src/main/resources/profiles/dev.properties`

</details>

<details id="CWE-23_Relative_Path_Traversal">
<summary><b>CWE-23: Relative Path Traversal</b> — affected files</summary>

- `zheng-common/src/main/java/com/zheng/common/util/JarUtil.java`

</details>

<details id="CWE-477_Use_of_Obsolete_Function">
<summary><b>CWE-477: Use of Obsolete Function</b> — affected files</summary>

- `zheng-oss/zheng-oss-web/src/main/java/com/zheng/oss/web/service/AliyunOssService.java`
- `zheng-common/src/main/java/com/zheng/common/util/MybatisGeneratorUtil.java`

</details>

---

## Codebase Insights

> **Note:** These documents are generated by AI and may contain inaccuracies or incomplete information. Please review carefully.

> **Codebase Insights aren't available yet.**
>
> These documents are generated when assessment runs with **Full analysis** coverage. Re-run the assessment and set `analysisCoverage: full` to enable them.

[Share feedback](https://aka.ms/ghcp-appmod/feedback)

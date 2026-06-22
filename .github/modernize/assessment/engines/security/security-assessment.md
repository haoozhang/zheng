# Security Assessment Report

**Generated:** 2026-06-22T07:10:22.0000000Z

## Summary

| Metric | Count |
|--------|-------|
| Total Findings | 99 |
| CVE Vulnerabilities | 85 |
| CWE Vulnerabilities | 14 |
| Total Rules Assessed | 59 |
| Rules Passed | 45 |

### By Severity

| Severity | Count |
|----------|-------|
| mandatory | 88 |
| optional | 6 |
| potential | 5 |

### By Category

| Category | Count |
|----------|-------|
| CVE | 85 |
| Code Quality | 4 |
| Credentials & Secrets | 4 |
| File & Path Security | 3 |
| Injection Attacks | 3 |

## CVE Findings (Dependency Vulnerabilities)

### CVE-2026-49268: Apache Shiro: LDAP DN Injection in DefaultLdapRealm
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:85

[CVE-2026-49268](https://github.com/advisories/GHSA-x96m-rh44-vgv8): Apache Shiro: LDAP DN Injection in DefaultLdapRealm

Severity: HIGH

Affected dependencies:
  - org.apache.shiro:shiro-core:1.3.2 (declared at zheng-common/pom.xml:85)
  - org.apache.shiro:shiro-core:1.3.2 (declared at zheng-common/pom.xml:85)

Recommended fix:
  - Upgrade org.apache.shiro:shiro-core to 2.2.1 or later
  - Upgrade org.apache.shiro:shiro-core to 3.0.0-alpha-2 or later

### CVE-2025-70974: FASTJSON Includes Functionality from Untrusted Control Sphere 
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:284, zheng-message/zheng-message-sdk/pom.xml:27

[CVE-2025-70974](https://github.com/advisories/GHSA-jm7w-5684-pvh8): FASTJSON Includes Functionality from Untrusted Control Sphere 

Severity: CRITICAL

Affected dependencies:
  - com.alibaba:fastjson:1.2.28 (declared at zheng-common/pom.xml:284)
  - com.alibaba:fastjson:1.2.47 (declared at zheng-message/zheng-message-sdk/pom.xml:27)

Recommended fix:
  - Upgrade com.alibaba:fastjson to 1.2.48 or later

### CVE-2025-52999: jackson-core can throw a StackoverflowError when processing deeply nested data
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:289

[CVE-2025-52999](https://github.com/advisories/GHSA-h46c-h94j-95f3): jackson-core can throw a StackoverflowError when processing deeply nested data

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-core:2.9.9.3 (declared at zheng-common/pom.xml:289)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-core to 2.15.0 or later

### CVE-2025-48976: Apache Commons FileUpload, Apache Commons FileUpload: FileUpload DoS via part headers
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:201

[CVE-2025-48976](https://github.com/advisories/GHSA-vv7r-c36w-3prj): Apache Commons FileUpload, Apache Commons FileUpload: FileUpload DoS via part headers

Severity: HIGH

Affected dependencies:
  - commons-fileupload:commons-fileupload:1.3.3 (declared at zheng-common/pom.xml:201)

Recommended fix:
  - Upgrade commons-fileupload:commons-fileupload to 1.6.0 or later

### CVE-2025-48734: Apache Commons Improper Access Control vulnerability
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:218

[CVE-2025-48734](https://github.com/advisories/GHSA-wxr5-93ph-8wr9): Apache Commons Improper Access Control vulnerability

Severity: HIGH

Affected dependencies:
  - commons-beanutils:commons-beanutils:1.9.3 (declared at zheng-common/pom.xml:218)

Recommended fix:
  - Upgrade commons-beanutils:commons-beanutils to 1.11.0 or later

### CVE-2024-38819: Spring Framework Path Traversal vulnerability
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:47

[CVE-2024-38819](https://github.com/advisories/GHSA-g5vr-rgqm-vf78): Spring Framework Path Traversal vulnerability

Severity: HIGH

Affected dependencies:
  - org.springframework:spring-webmvc:4.3.20.RELEASE (declared at zheng-common/pom.xml:47)
  - org.springframework:spring-webmvc:4.3.20.RELEASE (declared at zheng-common/pom.xml:47)
  - org.springframework:spring-webmvc:4.3.20.RELEASE (declared at zheng-common/pom.xml:47)

Recommended fix:
  - Upgrade org.springframework:spring-webmvc to 6.1.14 or later

### CVE-2023-22102: MySQL Connectors takeover vulnerability
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:167

[CVE-2023-22102](https://github.com/advisories/GHSA-m6vm-37g8-gqvh): MySQL Connectors takeover vulnerability

Severity: HIGH

Affected dependencies:
  - mysql:mysql-connector-java:5.1.34 (declared at zheng-common/pom.xml:167)

### CVE-2023-34478: Path Traversal in Apache Shiro
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:90

[CVE-2023-34478](https://github.com/advisories/GHSA-pmhc-2g4f-85cg): Path Traversal in Apache Shiro

Severity: CRITICAL

Affected dependencies:
  - org.apache.shiro:shiro-web:1.3.2 (declared at zheng-common/pom.xml:90)
  - org.apache.shiro:shiro-web:1.3.2 (declared at zheng-common/pom.xml:90)

Recommended fix:
  - Upgrade org.apache.shiro:shiro-web to 1.12.0 or later
  - Upgrade org.apache.shiro:shiro-web to 2.0.0-alpha-3 or later

### CVE-2023-24998: Apache Commons FileUpload denial of service vulnerability
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:201

[CVE-2023-24998](https://github.com/advisories/GHSA-hfrx-6qgj-fp6c): Apache Commons FileUpload denial of service vulnerability

Severity: HIGH

Affected dependencies:
  - commons-fileupload:commons-fileupload:1.3.3 (declared at zheng-common/pom.xml:201)

Recommended fix:
  - Upgrade commons-fileupload:commons-fileupload to 1.5 or later

### CVE-2022-40664: Apache Shiro Authentication Bypass vulnerability
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:85

[CVE-2022-40664](https://github.com/advisories/GHSA-45x9-q6vj-cqgq): Apache Shiro Authentication Bypass vulnerability

Severity: CRITICAL

Affected dependencies:
  - org.apache.shiro:shiro-core:1.3.2 (declared at zheng-common/pom.xml:85)

Recommended fix:
  - Upgrade org.apache.shiro:shiro-core to 1.10.0 or later

### CVE-2022-42003: Uncontrolled Resource Consumption in Jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2022-42003](https://github.com/advisories/GHSA-jjjh-jjxp-wpff): Uncontrolled Resource Consumption in Jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.12.7.1 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.13.4.2 or later

### CVE-2022-42004: Uncontrolled Resource Consumption in FasterXML jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2022-42004](https://github.com/advisories/GHSA-rgv9-q543-rqg4): Uncontrolled Resource Consumption in FasterXML jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.13.4 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.12.7.1 or later

### CVE-2020-10650: jackson-databind vulnerable to unsafe deserialization
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-10650](https://github.com/advisories/GHSA-rpr3-cw39-3pxh): jackson-databind vulnerable to unsafe deserialization

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later

### CVE-2022-32532: Improper Authorization in Apache Shiro
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:85

[CVE-2022-32532](https://github.com/advisories/GHSA-4cf5-xmhp-3xj7): Improper Authorization in Apache Shiro

Severity: CRITICAL

Affected dependencies:
  - org.apache.shiro:shiro-core:1.3.2 (declared at zheng-common/pom.xml:85)

Recommended fix:
  - Upgrade org.apache.shiro:shiro-core to 1.9.1 or later

### CVE-2022-25845: Unsafe deserialization in com.alibaba:fastjson
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:284, zheng-message/zheng-message-sdk/pom.xml:27

[CVE-2022-25845](https://github.com/advisories/GHSA-pv7h-hx5h-mgfj): Unsafe deserialization in com.alibaba:fastjson

Severity: HIGH

Affected dependencies:
  - com.alibaba:fastjson:1.2.28 (declared at zheng-common/pom.xml:284)
  - com.alibaba:fastjson:1.2.47 (declared at zheng-message/zheng-message-sdk/pom.xml:27)

Recommended fix:
  - Upgrade com.alibaba:fastjson to 1.2.83 or later

### CVE-2018-3258: Improper Privilege Management in MySQL Connectors Java
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:167

[CVE-2018-3258](https://github.com/advisories/GHSA-4vrv-ch96-6h42): Improper Privilege Management in MySQL Connectors Java

Severity: HIGH

Affected dependencies:
  - mysql:mysql-connector-java:5.1.34 (declared at zheng-common/pom.xml:167)

Recommended fix:
  - Upgrade mysql:mysql-connector-java to 8.0.13 or later

### CVE-2017-3523: Improper Access Control in MySQL Connectors Java
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:167

[CVE-2017-3523](https://github.com/advisories/GHSA-2xxh-f8r3-hvvr): Improper Access Control in MySQL Connectors Java

Severity: HIGH

Affected dependencies:
  - mysql:mysql-connector-java:5.1.34 (declared at zheng-common/pom.xml:167)

Recommended fix:
  - Upgrade mysql:mysql-connector-java to 5.1.41 or later

### CVE-2022-28111: MyBatis PageHelper vulnerable to time-blind SQL injection via orderBy parameter
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:116

[CVE-2022-28111](https://github.com/advisories/GHSA-w559-623p-vfg8): MyBatis PageHelper vulnerable to time-blind SQL injection via orderBy parameter

Severity: CRITICAL

Affected dependencies:
  - com.github.pagehelper:pagehelper:5.0.1 (declared at zheng-common/pom.xml:116)

Recommended fix:
  - Upgrade com.github.pagehelper:pagehelper to 5.3.1 or later

### CVE-2022-22965: Remote Code Execution in Spring Framework
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:47

[CVE-2022-22965](https://github.com/advisories/GHSA-36p3-wjmg-h94x): Remote Code Execution in Spring Framework

Severity: CRITICAL

Affected dependencies:
  - org.springframework:spring-webmvc:4.3.20.RELEASE (declared at zheng-common/pom.xml:47)
  - org.springframework:spring-webmvc:4.3.20.RELEASE (declared at zheng-common/pom.xml:47)

Recommended fix:
  - Upgrade org.springframework:spring-webmvc to 5.3.18 or later
  - Upgrade org.springframework:spring-webmvc to 5.2.20.RELEASE or later

### CVE-2020-36518: Deeply nested json in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-36518](https://github.com/advisories/GHSA-57j2-w4cx-62h2): Deeply nested json in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.13.2.1 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.12.6.1 or later

### CVE-2020-17523: Authentication bypass in Apache Shiro
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:90, zheng-common/pom.xml:100

[CVE-2020-17523](https://github.com/advisories/GHSA-v98j-7crc-wvrj): Authentication bypass in Apache Shiro

Severity: CRITICAL

Affected dependencies:
  - org.apache.shiro:shiro-web:1.3.2 (declared at zheng-common/pom.xml:90)
  - org.apache.shiro:shiro-spring:1.3.2 (declared at zheng-common/pom.xml:100)

Recommended fix:
  - Upgrade org.apache.shiro:shiro-web to 1.7.1 or later
  - Upgrade org.apache.shiro:shiro-spring to 1.7.1 or later

### CVE-2020-13936: Sandbox Bypass in Apache Velocity Engine
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:144

[CVE-2020-13936](https://github.com/advisories/GHSA-59j4-wjwp-mw9m): Sandbox Bypass in Apache Velocity Engine

Severity: HIGH

Affected dependencies:
  - org.apache.velocity:velocity:1.7 (declared at zheng-common/pom.xml:144)

### CVE-2020-36189: Unsafe Deserialization in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-36189](https://github.com/advisories/GHSA-vfqx-33qm-g869): Unsafe Deserialization in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.5 or later

### CVE-2020-36187: Unsafe Deserialization in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-36187](https://github.com/advisories/GHSA-r695-7vr9-jgc2): Unsafe Deserialization in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later

### CVE-2020-36188: Unsafe Deserialization in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-36188](https://github.com/advisories/GHSA-f9xh-2qgp-cq57): Unsafe Deserialization in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.5 or later

### CVE-2020-36183: Unsafe Deserialization in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-36183](https://github.com/advisories/GHSA-9m6f-7xcq-8vf8): Unsafe Deserialization in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.5 or later

### CVE-2020-36184: Unsafe Deserialization in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-36184](https://github.com/advisories/GHSA-m6x4-97wx-4q27): Unsafe Deserialization in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later

### CVE-2020-36180: Unsafe Deserialization in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-36180](https://github.com/advisories/GHSA-8c4j-34r4-xr8g): Unsafe Deserialization in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.5 or later

### CVE-2020-36181: Unsafe Deserialization in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-36181](https://github.com/advisories/GHSA-cvm9-fjm9-3572): Unsafe Deserialization in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.5 or later

### CVE-2020-36185: Unsafe Deserialization in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-36185](https://github.com/advisories/GHSA-8w26-6f25-cm9x): Unsafe Deserialization in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later

### CVE-2020-36179: Unsafe Deserialization in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-36179](https://github.com/advisories/GHSA-9gph-22xh-8x98): Unsafe Deserialization in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.5 or later

### CVE-2020-36182: Unsafe Deserialization in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-36182](https://github.com/advisories/GHSA-89qr-369f-5m5x): Unsafe Deserialization in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.5 or later

### CVE-2020-24750: Unsafe Deserialization in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-24750](https://github.com/advisories/GHSA-qjw2-hr98-qgfh): Unsafe Deserialization in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.5 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.6 or later

### CVE-2020-35728: Serialization gadget exploit in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-35728](https://github.com/advisories/GHSA-5r5r-6hpj-8gg9): Serialization gadget exploit in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later

### CVE-2020-35491: Serialization gadgets exploit in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-35491](https://github.com/advisories/GHSA-r3gr-cxrf-hg25): Serialization gadgets exploit in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later

### CVE-2020-35490: Serialization gadgets exploit in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-35490](https://github.com/advisories/GHSA-wh8g-3j2c-rqj5): Serialization gadgets exploit in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later

### CVE-2020-24616: Code Injection in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-24616](https://github.com/advisories/GHSA-h3cw-g4mq-c5x2): Code Injection in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.6 or later

### CVE-2020-36186: Unsafe Deserialization in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-36186](https://github.com/advisories/GHSA-v585-23hc-c647): Unsafe Deserialization in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.8 or later

### CVE-2021-41303: Apache Shiro vulnerable to a specially crafted HTTP request causing an authentication bypass
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:85

[CVE-2021-41303](https://github.com/advisories/GHSA-f6jp-j6w3-w9hm): Apache Shiro vulnerable to a specially crafted HTTP request causing an authentication bypass

Severity: CRITICAL

Affected dependencies:
  - org.apache.shiro:shiro-core:1.3.2 (declared at zheng-common/pom.xml:85)

Recommended fix:
  - Upgrade org.apache.shiro:shiro-core to 1.8.0 or later

### CVE-2021-36090: Improper Handling of Length Parameter Inconsistency in Compress
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:233

[CVE-2021-36090](https://github.com/advisories/GHSA-mc84-pj99-q6hh): Improper Handling of Length Parameter Inconsistency in Compress

Severity: HIGH

Affected dependencies:
  - org.apache.commons:commons-compress:1.18 (declared at zheng-common/pom.xml:233)

Recommended fix:
  - Upgrade org.apache.commons:commons-compress to 1.21 or later

### CVE-2021-35517: Improper Handling of Length Parameter Inconsistency in Compress
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:233

[CVE-2021-35517](https://github.com/advisories/GHSA-xqfj-vm6h-2x34): Improper Handling of Length Parameter Inconsistency in Compress

Severity: HIGH

Affected dependencies:
  - org.apache.commons:commons-compress:1.18 (declared at zheng-common/pom.xml:233)

Recommended fix:
  - Upgrade org.apache.commons:commons-compress to 1.21 or later

### CVE-2021-35516: Improper Handling of Length Parameter Inconsistency in Compress
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:233

[CVE-2021-35516](https://github.com/advisories/GHSA-crv7-7245-f45f): Improper Handling of Length Parameter Inconsistency in Compress

Severity: HIGH

Affected dependencies:
  - org.apache.commons:commons-compress:1.18 (declared at zheng-common/pom.xml:233)

Recommended fix:
  - Upgrade org.apache.commons:commons-compress to 1.21 or later

### CVE-2021-35515: Excessive Iteration in Compress
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:233

[CVE-2021-35515](https://github.com/advisories/GHSA-7hfm-57qf-j43q): Excessive Iteration in Compress

Severity: HIGH

Affected dependencies:
  - org.apache.commons:commons-compress:1.18 (declared at zheng-common/pom.xml:233)

Recommended fix:
  - Upgrade org.apache.commons:commons-compress to 1.21 or later

### CVE-2020-13933: Authentication bypass in Apache Shiro
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:85

[CVE-2020-13933](https://github.com/advisories/GHSA-2vgm-wxr3-6w2j): Authentication bypass in Apache Shiro

Severity: HIGH

Affected dependencies:
  - org.apache.shiro:shiro-core:1.3.2 (declared at zheng-common/pom.xml:85)

Recommended fix:
  - Upgrade org.apache.shiro:shiro-core to 1.6.0 or later

### CVE-2020-1957: Improper Authentication in Apache Shiro
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:85

[CVE-2020-1957](https://github.com/advisories/GHSA-26gr-cvq3-qxgf): Improper Authentication in Apache Shiro

Severity: CRITICAL

Affected dependencies:
  - org.apache.shiro:shiro-core:1.3.2 (declared at zheng-common/pom.xml:85)

Recommended fix:
  - Upgrade org.apache.shiro:shiro-core to 1.5.2 or later

### CVE-2020-11989: Improper Authentication in Apache Shiro
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:85

[CVE-2020-11989](https://github.com/advisories/GHSA-72w9-fcj5-3fcg): Improper Authentication in Apache Shiro

Severity: CRITICAL

Affected dependencies:
  - org.apache.shiro:shiro-core:1.3.2 (declared at zheng-common/pom.xml:85)

Recommended fix:
  - Upgrade org.apache.shiro:shiro-core to 1.5.3 or later

### CVE-2020-26945: "Deserialization errors in MyBatis"
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:106

[CVE-2020-26945](https://github.com/advisories/GHSA-qq48-m4jx-xqh8): "Deserialization errors in MyBatis"

Severity: HIGH

Affected dependencies:
  - org.mybatis:mybatis:3.4.2 (declared at zheng-common/pom.xml:106)

Recommended fix:
  - Upgrade org.mybatis:mybatis to 3.5.6 or later

### CVE-2020-17510: Authentication bypass in Apache Shiro
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:100

[CVE-2020-17510](https://github.com/advisories/GHSA-7cj4-gj8m-m2f7): Authentication bypass in Apache Shiro

Severity: CRITICAL

Affected dependencies:
  - org.apache.shiro:shiro-spring:1.3.2 (declared at zheng-common/pom.xml:100)

Recommended fix:
  - Upgrade org.apache.shiro:shiro-spring to 1.7.0 or later

### CVE-2020-25649: XML External Entity (XXE) Injection in Jackson Databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-25649](https://github.com/advisories/GHSA-288c-cq4h-88gq): XML External Entity (XXE) Injection in Jackson Databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.7 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.10.5.1 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.4 or later

### CVE-2021-20190: Deserialization of untrusted data in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2021-20190](https://github.com/advisories/GHSA-5949-rw7g-wx7w): Deserialization of untrusted data in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.7 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.5 or later

### CVE-2020-14061: Deserialization of untrusted data in Jackson Databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-14061](https://github.com/advisories/GHSA-c2q3-4qrh-fm48): Deserialization of untrusted data in Jackson Databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.5 or later

### CVE-2020-14062: Deserialization of untrusted data in Jackson Databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-14062](https://github.com/advisories/GHSA-c265-37vj-cwcc): Deserialization of untrusted data in Jackson Databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.5 or later

### CVE-2020-14060: Deserialization of untrusted data in Jackson Databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-14060](https://github.com/advisories/GHSA-j823-4qch-3rgm): Deserialization of untrusted data in Jackson Databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.5 or later

### CVE-2020-14195: Deserialization of untrusted data in Jackson Databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-14195](https://github.com/advisories/GHSA-mc6h-4qgp-37qh): Deserialization of untrusted data in Jackson Databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.5 or later

### CVE-2019-10086: Insecure Deserialization in Apache Commons Beanutils
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:218

[CVE-2019-10086](https://github.com/advisories/GHSA-6phf-73q6-gh87): Insecure Deserialization in Apache Commons Beanutils

Severity: HIGH

Affected dependencies:
  - commons-beanutils:commons-beanutils:1.9.3 (declared at zheng-common/pom.xml:218)

Recommended fix:
  - Upgrade commons-beanutils:commons-beanutils to 1.9.4 or later

### CVE-2017-7536: Privilege Escalation in Hibernate Validator
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:254

[CVE-2017-7536](https://github.com/advisories/GHSA-xxgp-pcfc-3vgc): Privilege Escalation in Hibernate Validator

Severity: HIGH

Affected dependencies:
  - org.hibernate:hibernate-validator:5.2.2.Final (declared at zheng-common/pom.xml:254)
  - org.hibernate:hibernate-validator:5.2.2.Final (declared at zheng-common/pom.xml:254)
  - org.hibernate:hibernate-validator:5.2.2.Final (declared at zheng-common/pom.xml:254)

Recommended fix:
  - Upgrade org.hibernate:hibernate-validator to 5.2.5.Final or later
  - Upgrade org.hibernate:hibernate-validator to 5.3.6.Final or later
  - Upgrade org.hibernate:hibernate-validator to 5.4.2.Final or later

### CVE-2019-17267: Improper Input Validation in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2019-17267](https://github.com/advisories/GHSA-f3j5-rmmp-3fc5): Improper Input Validation in jackson-databind

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.8.11.5 or later

### CVE-2014-0114: Arbitrary code execution in Apache Commons BeanUtils
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:218

[CVE-2014-0114](https://github.com/advisories/GHSA-p66x-2cv9-qq3v): Arbitrary code execution in Apache Commons BeanUtils

Severity: HIGH

Affected dependencies:
  - commons-beanutils:commons-beanutils:1.9.3 (declared at zheng-common/pom.xml:218)

Recommended fix:
  - Upgrade commons-beanutils:commons-beanutils to 1.9.4 or later

### CVE-2020-11112: jackson-databind mishandles the interaction between serialization gadgets and typing
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-11112](https://github.com/advisories/GHSA-58pp-9c76-5625): jackson-databind mishandles the interaction between serialization gadgets and typing

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later

### CVE-2020-9547: jackson-databind mishandles the interaction between serialization gadgets and typing
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-9547](https://github.com/advisories/GHSA-q93h-jc49-78gg): jackson-databind mishandles the interaction between serialization gadgets and typing

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.8.11.6 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.7.9.7 or later

### CVE-2019-14893: Polymorphic deserialization of malicious object in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2019-14893](https://github.com/advisories/GHSA-qmqc-x3r4-6v39): Polymorphic deserialization of malicious object in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10 or later

### CVE-2020-10673: jackson-databind mishandles the interaction between serialization gadgets and typing
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-10673](https://github.com/advisories/GHSA-fqwf-pjwf-7vqv): jackson-databind mishandles the interaction between serialization gadgets and typing

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.4 or later

### CVE-2020-9548: jackson-databind mishandles the interaction between serialization gadgets and typing
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-9548](https://github.com/advisories/GHSA-p43x-xfjf-5jhr): jackson-databind mishandles the interaction between serialization gadgets and typing

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.8.11.6 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.7.9.7 or later

### CVE-2019-14892: Polymorphic deserialization of malicious object in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2019-14892](https://github.com/advisories/GHSA-cf6r-3wgc-h863): Polymorphic deserialization of malicious object in jackson-databind

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.3 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.8.11.5 or later

### CVE-2020-10968: jackson-databind mishandles the interaction between serialization gadgets and typing
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-10968](https://github.com/advisories/GHSA-rf6r-2c4q-2vwg): jackson-databind mishandles the interaction between serialization gadgets and typing

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later

### CVE-2020-11111: jackson-databind mishandles the interaction between serialization gadgets and typing
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-11111](https://github.com/advisories/GHSA-v3xw-c963-f5hc): jackson-databind mishandles the interaction between serialization gadgets and typing

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later

### CVE-2020-11113: jackson-databind mishandles the interaction between serialization gadgets and typing
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-11113](https://github.com/advisories/GHSA-9vvp-fxw6-jcxr): jackson-databind mishandles the interaction between serialization gadgets and typing

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later

### CVE-2020-11619: jackson-databind mishandles the interaction between serialization gadgets and typing
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-11619](https://github.com/advisories/GHSA-27xj-rqx5-2255): jackson-databind mishandles the interaction between serialization gadgets and typing

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later

### CVE-2020-10969: jackson-databind mishandles the interaction between serialization gadgets and typing
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-10969](https://github.com/advisories/GHSA-758m-v56v-grj4): jackson-databind mishandles the interaction between serialization gadgets and typing

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later

### CVE-2020-9546: jackson-databind mishandles the interaction between serialization gadgets and typing
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-9546](https://github.com/advisories/GHSA-5p34-5m6p-p58g): jackson-databind mishandles the interaction between serialization gadgets and typing

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later

### CVE-2020-11620: jackson-databind mishandles the interaction between serialization gadgets and typing
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-11620](https://github.com/advisories/GHSA-h4rc-386g-6m85): jackson-databind mishandles the interaction between serialization gadgets and typing

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later

### CVE-2020-10672: jackson-databind mishandles the interaction between serialization gadgets and typing
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-10672](https://github.com/advisories/GHSA-95cm-88f5-f2c7): jackson-databind mishandles the interaction between serialization gadgets and typing

Severity: HIGH

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.4 or later

### CVE-2020-8840: Deserialization of Untrusted Data in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2020-8840](https://github.com/advisories/GHSA-4w82-r329-3q67): Deserialization of Untrusted Data in jackson-databind

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.7.9.7 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.8.11.5 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.3 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.4 or later

### CVE-2019-20330: Deserialization of Untrusted Data in jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2019-20330](https://github.com/advisories/GHSA-gww7-p5w4-wrfv): Deserialization of Untrusted Data in jackson-databind

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.7.9.7 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.8.11.5 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.2 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.4 or later

### CVE-2019-12422: Improper input validation in Apache Shiro
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:85

[CVE-2019-12422](https://github.com/advisories/GHSA-r679-m633-g7wc): Improper input validation in Apache Shiro

Severity: HIGH

Affected dependencies:
  - org.apache.shiro:shiro-core:1.3.2 (declared at zheng-common/pom.xml:85)

Recommended fix:
  - Upgrade org.apache.shiro:shiro-core to 1.4.2 or later

### CVE-2019-17531: jackson-databind polymorphic typing issue
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2019-17531](https://github.com/advisories/GHSA-gjmw-vf9h-g25v): jackson-databind polymorphic typing issue

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.1 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.8.11.5 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.3 or later

### CVE-2019-16943: jackson-databind polymorphic typing issue
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2019-16943](https://github.com/advisories/GHSA-fmmc-742q-jg75): jackson-databind polymorphic typing issue

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.1 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.8.11.5 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.3 or later

### CVE-2019-16942: Polymorphic Typing in FasterXML jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2019-16942](https://github.com/advisories/GHSA-mx7p-6679-8g3q): Polymorphic Typing in FasterXML jackson-databind

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10.1 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.3 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.8.11.5 or later

### CVE-2019-12402: Denial of Service in Apache Commons Compress
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:233

[CVE-2019-12402](https://github.com/advisories/GHSA-53x6-4x5p-rrvv): Denial of Service in Apache Commons Compress

Severity: HIGH

Affected dependencies:
  - org.apache.commons:commons-compress:1.18 (declared at zheng-common/pom.xml:233)

Recommended fix:
  - Upgrade org.apache.commons:commons-compress to 1.19 or later

### CVE-2019-16335: Polymorphic Typing issue in FasterXML jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2019-16335](https://github.com/advisories/GHSA-85cw-hj65-qqv9): Polymorphic Typing issue in FasterXML jackson-databind

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.8.11.5 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.3 or later

### CVE-2019-14540: Polymorphic Typing issue in FasterXML jackson-databind
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:294

[CVE-2019-14540](https://github.com/advisories/GHSA-h822-r4r5-v8jg): Polymorphic Typing issue in FasterXML jackson-databind

Severity: CRITICAL

Affected dependencies:
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)
  - com.fasterxml.jackson.core:jackson-databind:2.9.9.3 (declared at zheng-common/pom.xml:294)

Recommended fix:
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.9.10 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.8.11.5 or later
  - Upgrade com.fasterxml.jackson.core:jackson-databind to 2.6.7.3 or later

### CVE-2026-22732: Spring Security HTTP Headers Are not Written Under Some Conditions
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:68

[CVE-2026-22732](https://github.com/advisories/GHSA-mf92-479x-3373): Spring Security HTTP Headers Are not Written Under Some Conditions

Severity: CRITICAL

Affected dependencies:
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)

Recommended fix:
  - Upgrade org.springframework.security:spring-security-web to 6.5.9 or later
  - Upgrade org.springframework.security:spring-security-web to 7.0.4 or later

### CVE-2024-38821: Spring Security vulnerable to Authorization Bypass of Static Resources in WebFlux Applications
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:68

[CVE-2024-38821](https://github.com/advisories/GHSA-c4q5-6c82-3qpw): Spring Security vulnerable to Authorization Bypass of Static Resources in WebFlux Applications

Severity: CRITICAL

Affected dependencies:
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)

Recommended fix:
  - Upgrade org.springframework.security:spring-security-web to 5.7.13 or later
  - Upgrade org.springframework.security:spring-security-web to 5.8.15 or later
  - Upgrade org.springframework.security:spring-security-web to 6.2.7 or later
  - Upgrade org.springframework.security:spring-security-web to 6.0.13 or later
  - Upgrade org.springframework.security:spring-security-web to 6.1.11 or later
  - Upgrade org.springframework.security:spring-security-web to 6.3.4 or later

### CVE-2022-22978: Authorization bypass in Spring Security
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:68

[CVE-2022-22978](https://github.com/advisories/GHSA-hh32-7344-cg2f): Authorization bypass in Spring Security

Severity: CRITICAL

Affected dependencies:
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)

Recommended fix:
  - Upgrade org.springframework.security:spring-security-web to 5.5.7 or later
  - Upgrade org.springframework.security:spring-security-web to 5.6.4 or later
  - Upgrade org.springframework.security:spring-security-web to 5.4.11 or later

### CVE-2021-22112: Privilege escalation in spring security
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** zheng-common/pom.xml:68

[CVE-2021-22112](https://github.com/advisories/GHSA-gq28-h5vg-8prx): Privilege escalation in spring security

Severity: HIGH

Affected dependencies:
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)
  - org.springframework.security:spring-security-web:4.2.8.RELEASE (declared at zheng-common/pom.xml:68)

Recommended fix:
  - Upgrade org.springframework.security:spring-security-web to 5.2.9 or later
  - Upgrade org.springframework.security:spring-security-web to 5.4.4 or later
  - Upgrade org.springframework.security:spring-security-web to 5.3.8 or later

## CWE Findings (Code-Level Vulnerabilities)

### CWE-477: Use of Obsolete Function
- **Category:** Code Quality
- **Severity:** optional
- **Story Points:** 1
- **Files:** zheng-oss/zheng-oss-web/src/main/java/com/zheng/oss/web/service/AliyunOssService.java, zheng-common/src/main/java/com/zheng/common/util/MybatisGeneratorUtil.java

The non-thread-safe and obsolete `SimpleDateFormat` class is used in AliyunOssService.java (line 36) and MybatisGeneratorUtil.java (line 124). Java 8 introduced the thread-safe `DateTimeFormatter` and `java.time` API as replacements. Using `SimpleDateFormat` in a web application context (AliyunOssService is a Spring @Service) can cause data corruption under concurrent access.

### CWE-772: Missing Release of Resource after Effective Lifetime
- **Category:** Code Quality
- **Severity:** potential
- **Story Points:** 3
- **Files:** zheng-common/src/main/java/com/zheng/common/util/MybatisGeneratorUtil.java

In MybatisGeneratorUtil.generator() (around line 89), `jdbcUtil.release()` is invoked inside the try block but is not in a finally block. If `jdbcUtil.selectByParams()` (line 81) throws an exception, the database connection will not be released, causing a resource leak.

### CWE-775: Missing Release of File Descriptor or Handle after Effective Lifetime
- **Category:** Code Quality
- **Severity:** potential
- **Story Points:** 3
- **Files:** zheng-common/src/main/java/com/zheng/common/util/VelocityUtil.java

In VelocityUtil.generate() (lines 33-36), a `FileWriterWithEncoding writer` is created and closed manually with `writer.close()` (line 36), but the writer is not wrapped in a try-with-resources or a finally block. If `template.merge(context, writer)` throws an exception, the file writer will not be closed, causing a file descriptor leak.

### CWE-1057: Data Access Operations Outside of Expected Data Manager Component
- **Category:** Code Quality
- **Severity:** potential
- **Story Points:** 5
- **Files:** zheng-common/src/main/java/com/zheng/common/util/JdbcUtil.java, zheng-common/src/main/java/com/zheng/common/util/MybatisGeneratorUtil.java

The application uses MyBatis as its central data manager, but `JdbcUtil.java` performs raw JDBC operations (DriverManager.getConnection, PreparedStatement) bypassing the MyBatis layer. This utility is used by `MybatisGeneratorUtil.java` (line 80) to query database tables directly. Direct JDBC access outside the designated data manager violates the application's architectural design and can lead to inconsistent connection handling and security controls.

### CWE-259: Use of Hard-coded Password
- **Category:** Credentials & Secrets
- **Severity:** optional
- **Story Points:** 5
- **Files:** zheng-upms/zheng-upms-rpc-service/src/main/resources/profiles/dev.properties, zheng-common/src/main/java/com/zheng/common/util/AESUtil.java

Database passwords in dev.properties (e.g., `datasource.master.jdbc.****** are encrypted using AESUtil with the hard-coded key seed `ENCODE_RULES = "zheng"` (AESUtil.java line 19). Since the encryption key is embedded in the source code, anyone with access to the repository can trivially decrypt all stored credentials. The same pattern is repeated across all module dev.properties and prod.properties files.

### CWE-321: Use of Hard-coded Cryptographic Key
- **Category:** Credentials & Secrets
- **Severity:** potential
- **Story Points:** 5
- **Files:** zheng-common/src/main/java/com/zheng/common/util/AESUtil.java

In AESUtil.java (line 19), a static final field `ENCODE_RULES = "zheng"` is used as the seed for AES-128 key derivation via SHA1PRNG in `aesEncode()` and `aesDecode()` methods. This hard-coded key is used throughout the application to encrypt and decrypt all sensitive data including database passwords and API credentials. The key cannot be rotated without recompiling the application.

### CWE-778: Insufficient Logging
- **Category:** Credentials & Secrets
- **Severity:** potential
- **Story Points:** 3
- **Files:** zheng-upms/zheng-upms-server/src/main/java/com/zheng/upms/server/controller/SSOController.java

In SSOController.login() (lines 141-148), failed authentication attempts (UnknownAccountException, IncorrectCredentialsException, LockedAccountException) are returned as API response objects but are never logged via the declared LOGGER. Security-critical events like repeated login failures, locked account access attempts, and invalid username attempts are silently swallowed with no audit trail, making it impossible to detect brute-force attacks or account compromise.

### CWE-798: Use of Hard-coded Credentials
- **Category:** Credentials & Secrets
- **Severity:** optional
- **Story Points:** 5
- **Files:** zheng-common/src/main/java/com/zheng/common/util/AESUtil.java, zheng-upms/zheng-upms-rpc-service/src/main/resources/profiles/dev.properties

The AES encryption key `ENCODE_RULES = "zheng"` (AESUtil.java line 19) is hard-coded in source and is used to encrypt/decrypt all application credentials. Database passwords stored in profile .properties files (e.g., `rWd3Hb+AzNg3IXF1b5vD+g==`) are AES-encrypted with this known key, making them effectively hard-coded. The same AES utility is used to protect the generator JDBC passwords and Redis passwords across all modules.

### CWE-22: Improper Limitation of a Pathname to a Restricted Directory ('Path Traversal')
- **Category:** File & Path Security
- **Severity:** optional
- **Story Points:** 8
- **Files:** zheng-common/src/main/java/com/zheng/common/util/JarUtil.java

In JarUtil.decompress() (line 34), JAR entry names from untrusted archives are directly concatenated to the output path: `String outFileName = outputPath + je.getName()`. There is no validation that je.getName() does not contain path traversal sequences (e.g., '../../etc/passwd'), enabling a classic Zip Slip attack where a crafted archive can write files outside the intended output directory.

### CWE-23: Relative Path Traversal
- **Category:** File & Path Security
- **Severity:** optional
- **Story Points:** 5
- **Files:** zheng-common/src/main/java/com/zheng/common/util/JarUtil.java

In JarUtil.decompress() (line 34), relative path sequences (e.g., '../') embedded in JAR entry names are not neutralized before constructing the output file path. A malicious archive with entries like '../../evil.sh' would cause files to be written outside the intended output directory.

### CWE-434: Unrestricted Upload of File with Dangerous Type
- **Category:** File & Path Security
- **Severity:** mandatory
- **Story Points:** 8
- **Files:** zheng-oss/zheng-oss-web/src/main/java/com/zheng/oss/web/service/AliyunOssService.java

In AliyunOssService.policy() (lines 39-58), the Aliyun OSS upload policy only restricts file size (COND_CONTENT_LENGTH_RANGE) and key prefix (COND_KEY). There is no restriction on file type or MIME type, allowing users to upload any file type including dangerous types (e.g., .jsp, .sh, .exe) directly to the OSS bucket without validation.

### CWE-79: Improper Neutralization of Input During Web Page Generation ('Cross-site Scripting')
- **Category:** Injection Attacks
- **Severity:** optional
- **Story Points:** 8
- **Files:** zheng-ui/zheng-cms-web/blog/details/index.html, zheng-api/zheng-api-server/src/main/webapp/WEB-INF/jsp/403.jsp

Two XSS vulnerabilities found: (1) In blog/details/index.html (line 101), user-submitted comment content is rendered with Thymeleaf `th:utext` (`<dd th:each="comment : ${comments}" th:utext="${comment.content}">`) which outputs raw HTML without escaping, enabling stored XSS. Article content is also rendered unescaped (line 94). (2) In 403.jsp (lines 16,19), exception messages are output with unescaped JSP scriptlets `<%= e.getClass().getSimpleName()%>` and `<%= e.getMessage()%>`, enabling reflected XSS if attacker-controlled data appears in the exception message.

### CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')
- **Category:** Injection Attacks
- **Severity:** mandatory
- **Story Points:** 13
- **Files:** zheng-cms/zheng-cms-web/src/main/java/com/zheng/cms/web/controller/BlogController.java, zheng-cms/zheng-cms-web/src/main/java/com/zheng/cms/web/controller/SearchController.java, zheng-cms/zheng-cms-web/src/main/java/com/zheng/cms/web/controller/QaController.java

In BlogController.java (line 91), user-controlled @RequestParam values `sort` and `order` are directly concatenated and passed to MyBatis via `cmsArticleExample.setOrderByClause(sort + " " + order)`. MyBatis mapper XML uses `${orderByClause}` (string substitution, not parameterized), which injects the value verbatim into the SQL query. The same pattern appears in SearchController.java (line 52) and QaController.java (line 91). An attacker can manipulate the `sort` or `order` parameters to inject arbitrary SQL.

### CWE-502: Deserialization of Untrusted Data
- **Category:** Injection Attacks
- **Severity:** mandatory
- **Story Points:** 13
- **Files:** zheng-common/pom.xml

The application uses spring-session-data-redis:1.3.0.RELEASE (declared at zheng-common/pom.xml) which, by default, uses JDK Java serialization (JdkSerializationRedisSerializer) to store and retrieve session objects in Redis. If the Redis server is exposed or shared, an attacker who can write to Redis can store crafted serialized payloads that are deserialized by the application upon session access, leading to remote code execution. No custom serializer configuration (e.g., GenericJackson2JsonRedisSerializer) was found in the codebase.

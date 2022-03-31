---
title:  Gcp-Dns-Module
---

## 描述

GCP Dns-Module

## 参数说明


### 属性

 名称 | 描述 | 类型 | 是否必须 | 默认值 
 ------------ | ------------- | ------------- | ------------- | ------------- 
 project |  |  | true |  
 region |  |  | false |  
 service_account_file |  |  | false |  
 zone |  |  | false |  
 dns_name |  |  | true |  
 instance_ip_addr |  |  | true |  
 managed_zone |  |  | true |  
 writeConnectionSecretToRef | The secret which the cloud resource connection will be written to | [writeConnectionSecretToRef](#writeConnectionSecretToRef) | false |  


#### writeConnectionSecretToRef

 名称 | 描述 | 类型 | 是否必须 | 默认值 
 ------------ | ------------- | ------------- | ------------- | ------------- 
 name | The secret name which the cloud resource connection will be written to | string | true |  
 namespace | The secret namespace which the cloud resource connection will be written to | string | false |  
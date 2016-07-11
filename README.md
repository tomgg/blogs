### 项目测试环境
#### 编译发布
1. 编译OCRM
```bash
ssh aideploy@20.26.25.42; (aideploy/aideploy)
cd deploy_cscrm1/bin/;
sh create.sh;
```
2. 发布OCRM WEB APP INTER EXE PROD
```bash
ssh aideploy@20.26.25.42; (aideploy/aideploy)
cd deploy_cscrm1/bin;
sh deploy-crm-app-g1.sh;
sh deploy-crm-web-g1.sh;
sh deploy-inter.sh;
sh deploy-aicrm-exe.sh;
sh deploy-aiprod.sh
```
3. 发布OCRM CSF MSG
> 打开[jekins](http://20.26.20.106:8800/)页面   devops106/devops106
  点击 crm-center-qa 立即构建


#### 管理平台
[服务治理平台](http://20.26.25.40:8080/csf-admin/common/index.jsp)

[zookeeper](http://20.26.25.39:8080/zkWeb-1.0)

[marathon](http://20.26.25.11:8080)  账号/密码：dcosadmin/zjdcos01


#### 主机平台
```bash
ssh aiweb@20.26.25.131
ssh aiapp@20.26.25.132
ssh aiapp@20.26.25.133
ssh dcos@20.26.25.10
```

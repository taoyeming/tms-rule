# tms-rule

## 发布说明

### ios

ios部分是直接发布到了cocoapods的公有仓库, 可
1. 新创建账号
2. 更新版本，添加tag
3. 直接通过tms.podspec发布: `pod trunk push tms.podspec --allow-warnings --verbose`


### android

android部分是直接发布到了mavencentral,重新发布布置：
1. 需要注册sonatype 账号,完成新账号审核
2. 重新修改 `android/tms/publish-mavencentral.gradle`中参数 ,
3. 重新修改`android/tms/build.gradle`中修改对应版本信息，
4. 直接执行`android/tms/publish-mavencentral.gradle`完成发布。
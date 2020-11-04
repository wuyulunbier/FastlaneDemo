# FastlaneDemo

[fastlane官网](https://docs.fastlane.tools/)
[Jenkins](https://www.jenkins.io/)
[shell教程](https://www.runoob.com/linux/linux-shell.html)

fastlane的作用
fastlane帮你统一定义、运行、自动化你的app发布流程，并且可以和其他第三方工具如CocoaPods等很好的结合，也可以和其他第三方持续集成(Continuous Integration)工具如Jenkins等完美的结合

### fastlane常规用法

- 1 首先需要安装Ruby环境 
- 2 fastlane init 在项目路径下初始化fastlane
- 3 配置fastlane目录下的appfile和fastfile 
- 4 使用ruby编写自己的脚本


### 常规发布流程
 - 1  开发前，需要登录苹果开发者后台创建App、Provisioning Profiles、certificates等；
 - 2  使用Xcode开发，然后将上述相关文件和证书配置好；
 - 3  编译项目并自测；
 - 4  Archive项目；
 - 5  上传包到iTunes后台；
 - 6  配置TestFlight，准备测试刚上传的版本；
 - 7  发布测试版本；
 - 8  测试发现问题，重回2；
 - 9  测试完成，在iTunes后台提交版本截图、描述等信息；
 - 10 提交App Store审核；

### 目录结构
      Appfile:用于存储应用程序标识符和Apple ID 等信息
      Fastfile:配置管理 lane
      Deliverfile:将应用在 ITC 中的信息,统一配置在一个Deliverfile文件中，详见2.1
      metadata:功能同上也是配置应用在ITC中的信息,只不过是独立文本的形式配置的
      screenshots:包含截图数据


### flutter项目集成fastlane
   [fastlane](https://flutter.dev/docs/deployment/cd)

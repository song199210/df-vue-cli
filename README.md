# dfVue-cli
#### 这里只是利用webpack配置了vue单文件的运行环境；
>利用vue-cli脚手架开发项目有几个月了;vue-cli帮我们完成了0到1的过程，我们只要接着1往后走就OK了；
>闲下来之余就好奇0到1是怎样实现的；故花了点时间粗略的研究了下vue-cli配置文件；有些头绪，就整了个简单的；
>dfVue-cli项目中没有任何Demo，只是提供了很简单的Deom，主要让总结下怎样配置vue脚手架运行环境；

### 第一步：
通过npm install命令完成各依赖包的安装 ；如图所示<br/><br/>
<img src="https://github.com/song199210/dfVue-cli/blob/master/images/npmList.png" width="500px"/>
### 第二步：
配置webpack.config.js;这里只把webpack.config.js核心的部分给贴出来；如图所示<br/><br/>
<img src="https://github.com/song199210/dfVue-cli/blob/master/images/wkConf.png" width="500px"/>
<br/>注意：resolve中的alias配置一定要做的，否则会没效果的；
### 第三部：
在定义入口文件main.js时，我们一般都需要初始化vue实例，其中有个template属性，这也是必填项；主要用来替换挂载的DOM元素；

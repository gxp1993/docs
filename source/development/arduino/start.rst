<h1 id="w600-arduino-入门教程">W600 Arduino 入门教程</h1>
<h2 id="简介">1.简介</h2>
<p><a href="https://baike.baidu.com/item/Arduino">Arduino</a>是一款便捷灵活、方便上手的开源电子原型平台。</p>
<p>W600 与 Arduino 的结合，使得W600继承了Arduino的开放性、易用性、交流性、丰富的第三方资源，更便捷的支持开发者进行自己的产品设计。</p>
<h2 id="准备工作">2.准备工作</h2>
<ul>
<li>arduino开发包</li>
<li>TB-01开发板</li>
</ul>
<h2 id="环境搭建">3. 环境搭建</h2>
<h3 id="下载arduino-ide">3.1 下载arduino ide</h3>
<p>这个就不赘述了，不知道的百度一下即可</p>
<h3 id="创建项目文件夹">3.2 创建项目文件夹</h3>
<p>创建一个文件夹 arudino，将下载的arduino开发包解压再该文件夹内，注意次级目录必须为hardware.</p>
<p>参考：</p>
<figure>
<img src="C:\Users\17118\Documents\DOCS\arduino\Untitled.assets\1545994646838.png" alt="1545994646838" /><figcaption>1545994646838</figcaption>
</figure>
<h3 id="设置项目文件夹">3.3 设置项目文件夹</h3>
<p>打开Arudion IDE，点击 文件，点击 首选项 。</p>
<figure>
<img src="C:\Users\17118\Documents\DOCS\arduino\Untitled.assets\1545994764034.png" alt="1545994764034" /><figcaption>1545994764034</figcaption>
</figure>
<h3 id="选择开发板">3.4 选择开发板</h3>
<p>配置完3.3步骤后，即可再开发板选项中选择</p>
<figure>
<img src="C:\Users\17118\Documents\DOCS\arduino\Untitled.assets\无标题-1545995025376.png" alt="无标题" /><figcaption>无标题</figcaption>
</figure>
<h3 id="测试demo">3.5 测试demo</h3>
<p>w600 arduino SDK提供了测试demo。</p>
<p>点击打开，选择 D:600600-arduino-0.1.0文件下的demo,进行测试。</p>
<p>此处选择 sketch_wifi_client 这个demo。</p>
<p>修改要连接的AP和SSID</p>
<p>static const char* ssid = “WX_ThingsTurn”;(修改成开发者实际要连接的热点) static const char* password = “thingsturn2018”;</p>
<p>点击编译、上传 即可。</p>
<p>注意！！！</p>
<ul>
<li>如果编译时出现弹窗，提示类似C++或者makeimg.exe 类似的错误，关闭IDE，以管理员模式运行。</li>
<li>该开发包时基于3.0SDK完成的，再上传固件之前，请先确认再第一次烧录arduino固件之前，模组内的固件为3.0版本SDK编译的固件，否则，请先烧录一下3.0版本SDK编译的固件，再上传，以免无法烧录固件</li>
</ul>

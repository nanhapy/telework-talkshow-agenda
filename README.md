# 关于远程工作的沟通方式与敏捷实践
## 远程工作概念
不受限于固定的工作时间和工作地点，通过网络进行沟通和协作的工作形式

## 远程工作优缺点
### 优点
  1. 对于企业：降低运营成本，房租/水电/网络/零食
  2. 对于客户：降低人力成本，美国企业雇佣中印员工/北京企业雇佣天津员工
  3. 对于员工：降低通勤成本，时间/交通费
  4. ...
### 劣势
1. 对于客户：
   1. 可把控性，不安全感。如何保证工作内容和工作量
   1. 甲方乙方的传统观念。
2. 对于企业：同客户
3. 对于员工：
   1. 自律（敏捷，以人为本）
   2. 工作与生活的界限
   3. 团队紧密度
4. 对于团队
   1. 沟通方式
   2. 项目管理

## 最佳实践

### 同事之间如何交流
1. 对方就一个问题和我描述了很多次，我还是没能理解他想表达什么……一个问题他怎么就说不明白呢。
   1. 保持一致的上下文。链接/Issues/聊天记录/代码段...
   2. 聊天记录，意外的财富。
   3. 不要试图只用文字消息来沟通。共享桌面/多媒体/视频...
2. 给对方发消息，等了很久还没回复……等待真的令人烦躁，他到底在干嘛？
   1. 提问测：
      1. 事情分轻重缓解，做好不能立刻回复的准备
      2. 实在紧急，打电话
   2. 应答侧：
      1. 半小时或者四十分钟的时间片段。起身休息，回复消息
      2. 即使没办法及时解决，也要及时回复。告诉他你的安排，“稍等10分钟”
3. 说好的开会讨论，怎么只有我一个人在发言……尴尬顺着网线传递过来，我好无力。
   1. 指名道姓，轮流发言
4. 我都下班了，怎么还有人给我消息。听到钉钉/Skype/Slack/微信/邮箱的新消息提醒我都有点精神衰弱了……
   1. 增加一次下班之前的站会，宣告你今天的工作结束。_不过这点我还没实现..._
   2. 国外有时差的情况，董老师是怎么办的？
5. 每个人都找我私聊，但是说的都是别人的事...就不能群组讨论吗
   1. 你们之间的谈话涉及到第三人称时，要注意可能需要建个群组来讨论了
   2. 别害羞，尽量在群里讨论

### 如何与客户交流
1. 保持沟通
   1. 与客户的项目负责人（产品经理/公司决策者）保持当前项目进度/未来项目计划的同步。
      1. 做到如果项目负责人的上司在问到他关于当前项目情况时，他不会毫无头绪。
   2. 与客户保持对重点业务/痛点业务/未来发展的同步
      1. 在你挖掘需求时，帮助你衡量需求的优先级
2. 80%的情况邮件即可解决
   1. 告知项目进度和项目计划。不能发送了事，必须收到确认
   2. 对于客户的咨询，尽量提供一种以上的方案，供其选择
3. 20%的情况需要语音通话
   1. 对于客户的质询，如不能胸有成竹，可以先挂断电话，收集信息，列提纲，待准备充分在回答。
      1.   为什么实现这个功能要花费这么长的时间？
      2.   为什么这个功能BUG这么多？
      3.   为什么服务总是挂掉？
      4.   ...   
4. 坚持原则与职业素养
   1. 勇于说不。不要为了赶工期尽快上线，放弃软件的可靠性和扩展性。

### 如何进行远程的敏捷开发
1. BackLog
   1. 需求挖掘
      1. 定期去客户现场
      2. 产品经理或者业务人员整理好，线上讨论
   2. 需求就是：为了达到怎样的商业目的，我们要怎么做。所以我们要考察一个需求：
      1. 这样做有没有达到目的
      2. 有没有更好的解决办法
      3. 从商业价值角度考量其价值
      4. 从未来发展角度考量其扩展性
      5. 从技术实现上考量其工作量
3. Sprint评审：任务细化/任务估时/任务分配/测试用例
   1. 远程会议
   2. 屏幕共享
   3. 轮流发言
4. 每日站会一早一晚
   1. 站会内容：可以谈论工作内容，也可以唠唠家常
   2. 理想的站会宣告了团队各成员的重叠工作时间
5. Code Review & Sprint Review 也可以线上进行
6. 工具：git/redmine/zeplin/蓝湖/云/cicd/容器技术栈/钉钉/zoom/slack...
7. Redmine使用示例
   1. 使用wiki文档或者知识库，记录重要需求
   2. 使用wiki文档，编写BackLog
   3. 使用路线图版本功能，创建Sprint
   4. 使用issues功能，创建细化后的任务，关联目标版本（Sprint），详细描述，预估时间
   5. 同时得到了Sprint的预估时间
   6. 使用更新issue状态，来模拟看板
   7. 使用issue登记工时，来填写工作日报
   8. 目标版本（Sprint）的issues如全部关闭，发布版本
   9. 导出目标版本（Sprint）的耗时，整理后，发给客户，完成工作内容和工作量的汇报
   10. 突发任务，建立issue，关联目标版本，来跟踪
   11. 缺点：
       1.  文档的通病，不更新不如没有。要保证有随时可以给人看文档的信心。
       2.  与代码版本控制关联较弱。提交只能通过issue号来关联

### 远程工作与现实生活
1. 让家人和同事清楚你上班与下班的界限
   1. 当你准备要在家工作时，你的女儿可能跑过来说要你陪他玩。你说，我要工作啦，下班一起玩。除非她哭了，摔了，生病了，你才会中断工作，去照顾他。**所以你需要给家人一个上班信号。** 这是相对容易的。
   2. 同样的，当你准备下班停止一天的工作，你的同事也可能来找你，会说有个问题还需要解决。你要说，我要下班啦，明天再解决吧。除非是紧急的，严重的，你才会放下手中的女儿去解决问题。**所以你需要给同事一个下班信号。** 这是相对不容易的。
   3. 让家人和同事清楚你上班与下班的界限，是对家人/同事的一种负责。
2. 让你自己保持线上与线下的平衡
   1. 工作是生活的一部分。除了远程工作外，还有各式各样的远程生活，比如网络游戏/视频通话等等，但：
      1. WOW是美好的，我也需要拥抱现实生活。
      2. 疫情期间，与女儿分隔两地已两月有余。即使每天视频一个小时，也远不及抱着她跳一支小曲。
   2. 现实生活有无可替代的魅力。和朋友一起吃饭，和家人一起出游。所以和同事一起去杵台球，打羽毛球，发现他们其他的优点和缺点。
   3. 让你自己保持线上与线下的平衡，是对自己和这个世界的一种负责。

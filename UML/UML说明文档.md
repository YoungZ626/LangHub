# UML说明文档
## 用例图说明
![ucd](https://github.com/nohack7/LangHub/blob/master/UML/LangHub_UML_UseCase.jpg "用例图")

我们的用例图中有两个参与者，分别为外语学习者和特约翻译官。
- 外语学习者的主要行为有登录、背单词、充值、翻译和社区交流。其中充值行为是拓展了账户管理行为。翻译行为包括两种——人工翻译和机器翻译。社区交流包括悬赏提问——包括提问、回答和采纳回答，以及发帖交流——包括发帖和回复。
- 特约翻译官的主要行为有登录、对翻译所得的提现和参与人工翻译。

![cd](https://github.com/nohack7/LangHub/blob/master/UML/LangHub_UML_CD.jpg)
## 类图说明
- 每个User对象包含ID、密码、账户余额、帖子列表、回复列表、单词列表属性，以及注册、登录登出、提问发帖、充值管理、学习单词等对应成员方法。
- 每个WordList对象由零个或多个Word对象组合而成，用户可进行自主增删操作。
- 每个Question对象包含作者ID、提问时间、内容、回复列表和采纳列表等属性，可对回复列表进行增删操作、并采纳回复列表中的元素加入采纳列表，用户可修改问题内容。
- 每个Answer对象包含作者ID、回复时间、采纳状态和回答内容等属性，用户可对回答内容进行修改。
- RewardPost类继承自Post类，增加了awardCoins属性。
- Community类包含一个questionList，可以对其进行增删改等操作。

## 顺序图
### 登录账户
![dl](https://github.com/nohack7/LangHub/blob/master/UML/%E7%99%BB%E5%BD%95%E9%A1%BA%E5%BA%8F%E5%9B%BE.jpg)

### 背单词
![recite](https://github.com/nohack7/LangHub/blob/master/UML/%E8%83%8C%E5%8D%95%E8%AF%8D%E9%A1%BA%E5%BA%8F%E5%9B%BE%20-.jpg)

### 翻译
![translate](https://github.com/nohack7/LangHub/blob/master/UML/%E7%BF%BB%E8%AF%91.jpg)

### 发帖
![post](https://github.com/nohack7/LangHub/blob/master/UML/%E5%8F%91%E5%B8%96%E9%A1%BA%E5%BA%8F%E5%9B%BE.png)

### 充值
![rc](https://github.com/nohack7/LangHub/blob/master/UML/%E5%85%85%E5%80%BC%E9%A1%BA%E5%BA%8F%E5%9B%BE.png)

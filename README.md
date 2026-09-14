# LLM-wiki
如何搭建个人知识库——LLM-wiki数据库搭建
# LLM-Wiki数据库搭建(一)

## 1. 为什么使用Obsidian？

> 个人知识库的搭建为什么使用Obsidian？明明有更多的选择，像Notion，印象笔记等等

**Obsidian**最大的优势在于

- 完全本地化，全部都是`md`文档，不怕云端的丢失
- 支持双向链接，可以方便的进行知识之间的关联
- 丰富的插件系统，多到你会忘记自己学习Obsidian的初衷

如何快速入手Obsidian，可以参考[Obsidian入门](https://mp.weixin.qq.com/s?__biz=Mzk0OTY3ODMzMg==&mid=2247484314&idx=1&sn=2aa125e5d5a8b60e2c756b02dca8a860&scene=21#wechat_redirect)

**Obsidian**最大的优势就是使用AI能自动帮你关联到相关的知识点和笔记；能够关联到相关的应用等方面，让你的知识不再是孤岛，而是连成一片



## 2. Claude Code最佳搭档

在[Claude Code](https://mp.weixin.qq.com/s?__biz=Mzk0OTY3ODMzMg==&mid=2247484109&idx=1&sn=23b494ac2614dd9e9a94c9b47c906cb9&scene=21#wechat_redirect)发展到现在之前，**Obsidian**就像VSCode一样，AI仅仅是作为插件辅助笔记的生成和管理，而Claude Code的出现，让Obsidian真正变成了一个AI时代下的知识库。

**Claude Code** 则是一个强大的 AI 编译器与自动化引擎。它能理解自然语言指令，读写本地文件系统，执行复杂的自动化任务。它的设计和 Obsidian 的本地存储模式天然契合——一个文件夹一个workspace

Claude Code与Obsidian结合，就像是VSCode与Git的结合，Claude Code负责AI的执行，Obsidian负责文档的存储和展示

- Obsidian 负责"结构化存储与可视化网络"
- Claude Code 负责"AI 编译与自动化管理"

> Obsidian是仓库，Claude是大脑，搭建成完整的思考系统

**系统优势：**

- 告别信息碎片化。 所有零散的信息都会被"编译"成相互关联的原子化知识单元
- 全流程自动化。 从信息收集、处理、分类、链接到结构化输出，大部分繁琐工作都由 AI 代劳，人适合做决策和判断
- 构建可生长的体系。 知识库不再是静态的仓库，而是一个能够通过 MOC（主题地图）和持续链接自我进化的有机体
- 成为高效"超级个体"。 知识高效转化为文章、报告、方案，提升个人输出与决策质量

### 3.1 Obsidian 安装

Obsidian的安装请查看这篇[安装教程和入门使用](https://mp.weixin.qq.com/s?__biz=Mzk0OTY3ODMzMg==&mid=2247484319&idx=1&sn=5a0fe108709ce34e131c2064323bba07&scene=21#wechat_redirect)，帮助你快速了Obsidian

### 3.2 Claude Code安装

Claude Code的安装和套餐API配置请看[claude code安装教程](https://mp.weixin.qq.com/s?__biz=Mzk0OTY3ODMzMg==&mid=2247484090&idx=1&sn=e580950d1abd4c14b7c8f4a45f8bedc7&scene=21#wechat_redirect),同样claude code使用，[skill使用](https://mp.weixin.qq.com/s?__biz=Mzk0OTY3ODMzMg==&mid=2247484120&idx=1&sn=73eb14365d972fa3b0c9e28ea865f6d8&scene=21#wechat_redirect)等等，请各自查看

传统的AI+笔记的方式，通常是

- 复制一段内容
- 打开网页/CHat客户端
- 让AI帮你总结、改写等
- 再粘贴回来

`Claude Code + Skills`:

- 调用技能 skills
- 能执行复杂指令(重写、拆解、结构化、补充)
- 作为你的协作伙伴，Claude 只是参与编辑，整理不改变你本身的原始数据

## 3.3 Claudian插件安装

> Obsidian最强大但同样最让人忘记初衷的地方就是插件市场

**在设置中选择第三方插件，然后关闭安全模式，即可打开三方插件市场**

![Image](D:\Typora\Typora\Markdown_image\640-1789387637261-18.png)

1. 手动安装

可以选择手动下载这些插件的安装包，然后手动放置在 obsidian 笔记仓库中的 `.obsidian/plugins` 文件夹下，这种比较繁琐，核心就是要放对位置

- 从github下载最新版本
- 创建文件夹，解压文件
- 复制到`.obsidian/plugins`目录下

1. **BRAT 插件安装**

BRAT全称Beta Reviewers Auto-update Tool（Beta测试者自动更新工具），是由开发者TfTHacker开发的Obsidian插件。

\> BRAT是一个专为开发者和插件/主题测试人员设计的插件，可以轻松安装测试版插件。通过将GitHub存储库路径添加到测试列表中，即可轻松检查更新，下载并重新加载插件，省去了手动创建文件夹、下载文件、复制到正确位置等繁琐步骤。该插件简化了测试过程，解决了开发者和测试人员的繁重工作，提高了工作效率。

在**[第三方市场插件](https://mp.weixin.qq.com/s?__biz=Mzk0OTY3ODMzMg==&mid=2247484374&idx=1&sn=ba583695b5dec778f37431358a714d91&scene=21#wechat_redirect)中**搜索`BRAT`，然后点击安装并启用即可，现在国内网络也能够成功安装插件了

![Image](D:\Typora\Typora\Markdown_image\640-1789387637261-19.png)

![Image](D:\Typora\Typora\Markdown_image\640-1789387637261-20.png)

安装好之后，最左侧会出现个笑脸，表示安装成功



1. **安装Claudian**

> Claudian 是一款能将 AI 编程智能体（比如 Claude Code、Codex，以及未来更多的工具）直接嵌入到你 Obsidian 库（Vault）中的插件。你的整个库会直接变成智能体的工作目录——这意味着文件读取与写入、内容搜索、运行 Bash 命令，以及多步骤的复杂工作流，全部都能开箱即用，无缝衔接

安装的方式有很多种:

```
1. 点击左侧笑脸-选择第一个install beta plugin 弹窗出现后在Repository窗口输入 https://github.com/YishenTu/claudian,然后点击`add plugin`即可

2. 在设置-第三方插件-BRAT，进入BRAT管理页面，然后找到Beta Plugin list，点击`Add beta plugin`，会同样弹出输入框，和第一种方法类似，把 https://github.com/YishenTu/claudian
```

![Image](D:\Typora\Typora\Markdown_image\640-1789387637261-21.png)

1. **激活Claude**

> 核心还是插件能够检测到`Claude CLI`否则是无法使用的

**安装Claude Code**:

- Linux/macOS/WSL2 安装可以参考之前的安装教程
- Windows用户下可以在`powershell`中，输入`& ([scriptblock]::Create((New-Object Net.WebClient).DownloadString("https://claude-zh.cn/scripts/install.ps1")))`，即可安装成功
- 安装成功后，直接在`C盘----用户----用户名`中找到`.claude`文件夹，新建`settings.json`文件，输入下面的内容，并把API Key填入即可(模型这里使用的智谱的，可使用该连接`https://www.bigmodel.cn/glm-coding?ic=TFCBPKTVRV`进行模型code plan的申请)

```
{
  "env": {
    "ANTHROPIC_AUTH_TOKEN": "",
    "ANTHROPIC_BASE_URL": "https://open.bigmodel.cn/api/anthropic",
    "API_TIMEOUT_MS": "3000000",
    "CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC": "1",
    "ANTHROPIC_DEFAULT_HAIKU_MODEL": "GLM-4.7",
    "ANTHROPIC_DEFAULT_SONNET_MODEL": "GLM-5",
    "ANTHROPIC_DEFAULT_OPUS_MODEL": "GLM-5.1"
  }
}
```

> 不管怎么样激活，都是需要系统先安装`Claude Code`，意味着Obsidian必须能够找到**Claude CLI**的安装,,添加环境变量主要作用只是修改`Claudian`的模型和显示

**Claudian现在已经支持Claude，CodeX和opencode三种平台**:

- 直接把系统中的`claude code`路径加上去,如果没能自己找到就需要手动添加

- 在环境(Enviroment)中添加一个新的环境，选择平台和输入API Key

  ![Image](D:\Typora\Typora\Markdown_image\640-1789387637262-22.png)

```
ANTHROPIC_API_TOKEN =   
ANTHROPIC_BASE_URL = https://open.bigmodel.cn/api/anthropic  
ANTHROPIC_DEFAULT_HAIKU_MODEL = glm-4.7
ANTHROPIC_DEFAULT_SONNET_MODEL = glm-5
ANTHROPIC_DEFAULT_OPUS_MODEL = glm-5.1
Claudian也好,BRAT也罢都是辅助的工具,核心还是要理解LLM的思想是什么,需要AI帮助人去做什么,即使是Claude Code中也能够使用,无非是便捷度的问题
```

![Image](D:\Typora\Typora\Markdown_image\640-1789387637262-23.png)

# LLM-Wiki数据库搭建(二)

## 4. 基础工具使用教程

按照上面的流程安装好`Obsidian`和`Claude Code`，以及`Claudian`插件之后，就可以开始搭建LLMWiki了，下面是一些核心的功能介绍和使用教程

> raw笔记 → LLM编译 → 结构化Wiki → 直接塞给LLM

**Claudian**包含的功能

- *Inline Edit（内联编辑）*： 选中文本或在光标位置使用快捷键，直接在笔记中进行编辑，并支持逐词级别的差异预览

- *Slash Commands & Skills（斜杠命令与技能）*：输入 `/`或 `$`，可调用可复用的提示模板或技能，支持用户级和知识库（vault）级作用域

  

- *`@mention（提及功能）`*: 输入 `@` 可以引用任何希望代理处理的内容，例如知识库文件、子代理、MCP 服务器或外部目录中的文件

- *Plan Mode规划模式*: 通过 `Shift + Tab` 切换。代理会先进行探索和设计，然后在执行前提交方案供你确认

- *Instruction Mode（指令模式 #）*

- *MCP Servers（MCP 服务器）*:通过 Model Context Protocol 连接外部工具（支持 stdio、SSE、HTTP）。Claude 在应用内管理知识库 MCP，Codex 使用其 CLI 管理 MCP 配置

- *Multi-Tab & Conversations（多标签与会话）*

### 4.1 基础使用方式

1. 点击 Obsidian 左侧功能区的`机器人头`图标,左侧会弹出`Claudian`的界面
2. 在笔记中**选中一段文字**，然后在右侧`claudian`进行编写
3. 会发现`Claudian`提醒选中的内容，你可以对选中的两行进行操作

![Image](D:\Typora\Typora\Markdown_image\640-1789387616634-6.png)

> AI 不再是“给你建议”，而是“直接帮你改文档”

### 4.2 SKILLs使用

只要合理使用`skills`,是能够最大化利用claude+obsidian：

- 重构一篇技术文章
- 拆解复杂概念
- 生成大纲 / TODO / 知识卡片
- 统一文档风格
- 把“零散笔记”整理成“系统知识”

> Claudian 最大的亮点之一，就是 完整支持 Claude Code 的 Skills

**安装Skills**一般有两种方式

1. 在obsidian打开的仓库中，显示所有的隐藏文件夹，找到`.claude`,点击进去，找到`skills`。比如要把Obsidian-skills https://github.com/kepano/obsidian-skills 安装到`Claudian`中，将`Obsidian-skills`zip文件下载解压之后，把skill中文件夹复制到`.claude/skills`中即可.当然插件中也能够自己编写skills

![Image](D:\Typora\Typora\Markdown_image\640-1789387616634-7.png)

> 相对于本地文件夹，坚果云这种云盘vault，可以把skill同步到每一个电脑



1. `Claudian`能够扫描本地`Claude Code`中的skill，主要是从`~/.claude/plugin`和 `~/.claude/skills`中扫描，所以也可通过claude code安装skill，从而得到`claudian`调用

![Image](D:\Typora\Typora\Markdown_image\640-1789387616634-8.png)

> 所有的skill使用和claude code中是一样的，`/skills names`即可调用

### 4.3 Obsidian web clipper使用

Obsidian web clipper是用来剪藏网页,当浏览到感兴趣的内容后,使用浏览器插件,或者在iOS safari中使用插件,一键将内容保存到自己的Obsidian 文件夹中,让你的知识不再凌乱,查找时不再忘了从哪里看到

- Obsidian web clipper安装请查看[[obsidian web clipper安装教程](https://mp.weixin.qq.com/s?__biz=Mzk0OTY3ODMzMg==&mid=2247484480&idx=1&sn=db55c6437ad2e70639fabb406c68eb74&scene=21#wechat_redirect)]
- Obsidian 网页剪藏器,阅读器,高亮,解释器,模板,变量,过滤器等使用,请查看[[相关介绍](https://mp.weixin.qq.com/s?__biz=Mzk0OTY3ODMzMg==&mid=2247484466&idx=1&sn=b6198259928ffbbba282e5bd90fdc39e&scene=21#wechat_redirect)]

![Image](D:\Typora\Typora\Markdown_image\640-1789387616634-9.png)

# LLM-Wiki数据库搭建(三)

## 5. LLM Wiki使用

LLM Wiki 是由 AI 先驱 Andrej Karpathy 提出的一种颠覆性个人知识管理范式。它摒弃了传统的 RAG（检索增强生成，即每次查询时从零查找拼接），转而让 AI 充当“全职笔记管理员”，将零散资料预先“编译”并持续更新为结构化、互相引用的 Markdown 维基百科

### 5.1 RAG的背景

过去两年，RAG（Retrieval-Augmented Generation）几乎成了 LLM 应用的"标配"。无论是企业知识库、智能客服还是个人笔记系统，大家的第一反应都是：把文档切块 → 向量化 → 存入向量数据库 → 查询时检索 → 拼进 Prompt。



```
文档/PDF/网页
        ↓
   文本提取
        ↓
  文本切分（Chunk）
        ↓
 Embedding模型
        ↓
   向量(Vector)
        ↓
 向量数据库存储
        ↓
  语义检索与问答
```

RAG流程缺陷:

- 分块损失：一篇结构化的论文，切成 512 token 的碎片后，上下文关系全丢了
- 检索不稳定：Embedding 相似度并不等于语义相关度，换个说法就可能检索不到
- 同一份文档，每次查询时 LLM 都要重新"阅读"原文，浪费算力
- 原始文档之间没有显式关联，知识只是"堆"在数据库里

> 简单理解就是: 把文件分解为向量存在向量库之后,每次查询都要重新阅读一遍,而且没有关联,只是堆在一起

### 5.2 LLM Wiki的背景

放弃查询时才从原始文档中检索的做法，让 LLM逐步构建和维护一个持久化的 wiki，一组结构化、相互链接的 Markdown 文件（一种轻量级的纯文本格式，可以用任何编辑器打开），作为你和原始资料之间的中间层。当你添加新资料时，LLM 不会只是把它索引起来留待日后检索，它会阅读、提取关键信息、整合进现有 wiki，更新实体页面、修订主题摘要、标注新数据与旧结论的矛盾之处、用新证据去强化或推翻已有的综合判断。知识被编译一次就沉淀下来、持续更新，不用每次查询时从头推导

> **wiki 是一个持久的、不断复利增长的产物**. LLM 负责编写和维护全部内容。人负责的是资料筛选、探索方向和提出正确的问题。LLM 做所有苦力活——总结、交叉引用、归档和 bookkeeping（指维护知识库一致性所需的大量琐碎更新工作，如同记账），这些工作才是让知识库随着时间推移真正有用的关键。

*Andrej Kaparthy* 举了几个简单的例子:

- 个人领域：追踪你自己的目标、健康、心理、自我提升——归档日记、文章、播客笔记，随着时间构建一幅关于你自己的结构化全景
- 研究领域：在数周或数月内深入一个课题——阅读论文、文章、报告，逐步构建一个带有演进论点的综合性 wiki。
- 阅读一本书：逐章归档，为人物、主题、情节线索建立页面，标注它们之间的关联。读完后你就拥有了一部丰富的伴读 wiki。
- 商业/团队：由 LLM 维护的内部 wiki，输入来源是 Slack 讨论、会议记录、项目文档、客户通话。可以有人类参与审核更新。wiki 之所以能保持更新，是因为 LLM 承担了团队中没人愿意做的维护工作。
- 竞争分析、尽职调查、旅行规划、课程笔记、爱好深挖——任何你在持续积累知识并希望它被组织起来而非散落各处的场景。

### 5.3 LLM Wiki 架构

**主要分成三层**

1. **原始资料源(Raw Sources)** -- 精心筛选的源文档集合。文章、论文、图片、数据文件。这些是只读的——LLM 从中读取但绝不修改，原始资料永远保持原样。这是你的权威来源

2. **Wiki** -- 一个由 LLM 生成的 Markdown 文件目录。摘要、实体页面、概念页面、对比分析、概览、综合判断。这一层完全由 LLM 拥有。它创建页面、在新资料到达时更新页面、维护交叉引用、保持一切一致, 你负责阅读，LLM 负责写。

3. **Schema（模式定义）** ——一份配置文档（例如 Claude Code 的 CLAUDE.md 或 OpenAI Codex 的 AGENTS.md——这些是各家 AI 编程工具的项目配置文件，告诉 AI 该遵循什么规则），定义 wiki 的结构是怎样的、约定是什么、在摄入资料、回答问题或维护 wiki 时应遵循什么工作流。这是关键配置文件——它让 LLM 成为一个有纪律的 wiki 维护者，而非一个通用聊天机器人。随着你对自己领域的理解加深，你和 LLM 会一起迭代这份文档，让它越来越好用。

   

### 5.4 LLM Wiki操作逻辑

- **摄入（Ingest）**: 你把新资料放进原始资料集，然后让 LLM 处理它。一个典型流程：LLM 阅读资料，与你讨论关键要点，在 wiki 中写一个摘要页面，更新索引，更新 wiki 中相关的实体和概念页面，并在日志中追加一条记录。一个资料源可能触及 10-15 个 wiki 页面. 个人偏好逐条摄入资料并全程参与——我读摘要、检查更新、引导 LLM 强调什么。但你也可以批量摄入大量资料，减少监督。怎么做取决于你自己，找到适合你的工作流后，记在 Schema 里，下次开新会话时 LLM 就能沿用
- **查询（Query）**: 你针对 wiki 提问。LLM 搜索相关页面、阅读它们、综合出带引用的答案。答案可以根据问题采取不同形式——一个 Markdown 页面、一个对比表格、一套幻灯片（Marp，一种把 Markdown 转成演示文稿的工具）、一张图表（matplotlib，Python 制图库）、一个画布。

> 好的答案可以作为新页面归档回 wiki, 请求的一次对比分析、一个分析结论、你发现的一个关联，这些都值得留下来，不应该消失在聊天历史中。这样，你的探索就像摄入的资料源一样，在知识库中实现复利增长

- **检查**（Lint——借用编程术语，原指代码静态检查工具，这里指对知识库做系统性的健康检查）。定期让 LLM 对 wiki 做健康检查。寻找：页面之间的矛盾、已被更新资料取代的过时论断、没有任何入站链接的孤儿页面（orphan pages，即没有其他页面链接到它的"孤岛"页面）、被提及但缺少独立页面的重要概念、缺失的交叉引用、可以通过网络搜索填补的数据缺口。LLM 擅长建议新的调查问题和新的资料来源。这让 wiki 在增长过程中保持健康。

> 随着Wiki的不断扩充，有两个特殊文件可以帮助LLM（以及您）更好地浏览Wiki。它们各有不同的用途

- **index.md**: 它是 wiki 中所有内容的目录——每个页面列出链接、一行摘要，以及可选的元数据（如日期或资料源计数）。按类别组织（实体、概念、资料源等）。LLM 在每次摄入时更新它。回答查询时，LLM 先读索引找到相关页面，再深入查看。这在中等规模（约 100 个资料源、数百个页面）下效果出奇地好，避免了基于 embedding（嵌入向量，一种把文本转成数字向量以便计算相似度的技术）的 RAG 基础设施的需求
- **log.md**: 它是一个只追加的记录（append-only，只增不改不删），记录发生了什么以及何时发生——摄入、查询、检查。一个实用技巧：如果每条记录以统一的前缀开头（例如## [2026-04-02] ingest | Article Title），日志就可以用简单的 Unix 命令行工具解析——`grep "^## \[" log.md | tail -5`就能给你最后 5 条记录。日志给你 wiki 演进的时间线，帮助 LLM 了解最近做了什么。

### 5.5 LLM wiki工具

后面介绍一下LLMwiki常用的工具,比如QMD是什么?为什么要用?怎么安装?怎么使用等,也会介绍桌面版的llm wiki软件;比较好用的LLM wiki skills有哪些,怎么用等

> 核心是理解思路,其他所有的变种都是按照原是数据库,AI处理后的wiki数据库,以及index,log文件组成

# LLM-Wiki数据库搭建(四)

### 5.5 LLM wiki工具

#### 5.5.1 QMD 搜索引擎

wiki 页面搜索引擎——在小规模下索引文件就够用了，但随着 wiki 增长，你需要正式的搜索能力。

- qmd 是个不错的选择：它是一个本地 Markdown 文件搜索引擎，支持 BM25/向量混合搜索（BM25 是经典的关键词匹配算法，向量搜索则通过语义相似度匹配，混合使用兼顾精确匹配和语义理解）和 LLM 重排序，全部在本地设备上运行

  ![Image](D:\Typora\Typora\Markdown_image\640-1789387575304-3.jpeg)

### 使用流程

#### 1. 安装

```
# 使用 npm
npm install -g @tobilu/qmd

# 或使用 Bun（更快）
bun install -g @tobilu/qmd

# 不想安装？直接用 npx 跑
npx @tobilu/qmd --version
```



#### 2. 创建集合

> `collection` 本质上是一个路径别名，方便后续搜索时指定范围。

```
# 索引你的笔记目录
qmd collection add ~/notes --name notes

# 再索引会议记录
qmd collection add ~/Documents/meetings --name meetings

# 查看已创建的集合
qmd collection list
```

#### 3. 添加上下文

> `context` 是搜索时使用的额外信息，例如当前日期、时间、地点、任务等。这些信息会自动添加到搜索结果中，帮助 LLM 更好地理解上下文。

```
# 告诉 QMD 这些目录是什么内容
qmd context add qmd://notes "个人笔记和技术想法"
qmd context add qmd://meetings "团队会议记录和决策"
```

#### 4. 生成嵌入

> 嵌入是为所有集合生成向量索引,首次运行会自动下载模式,缓存到本地,后续使用无需重复下载

```
qmd embed
```

#### 5. 搜索

```
# 关键词搜索（快，适合精确匹配）
qmd search "认证流程"

# 语义搜索（慢，但能理解你的意图）
qmd vsearch "用户怎么登录"

# 混合搜索（推荐，结合两者优势）
qmd query "季度规划会议说了什么" -c meetings

# 只看文件名，不显示具体内容
qmd query "错误处理" --files

# Get a specific document
qmd get "meetings/2024-01-15.md"

# Get a document by docid (shown in search results)
qmd get "#abc123"

# Get multiple documents by glob pattern
qmd multi-get "journals/2025-05*.md"

# Search within a specific collection
qmd search "API" -c notes

# Export all matches for an agent
qmd search "API" --all --files --min-score 0.3
```



### 实际使用

**将QMD搜索引擎链接AI才能发挥最大的功效**

> QMD 的 `--json` 和 `--files` 输出格式是为Agent工作流设计的

```
# Get structured results for an LLM 结构性输出
qmd search "authentication" --json -n 10

# List all relevant files above a threshold,设置一个阈值
qmd query "error handling" --all --files --min-score 0.4

# Retrieve full document content 返回所有满足条件的结果
qmd get "docs/api-reference.md" --full
```

1. **集成到Claude Code使用MCP**

虽然告诉AI在命令行中使用qmd即可运行,但是还是公开了一个MCP接口,方便集成到Claude Code中

*自动配置*

在终端命令行中执行下面的命令,安装插件系统

```
claude plugin marketplace add tobi/qmd
claude plugin install qmd@qmd
```

*手动配置*

在`~/.claude/settings.json`修改配置文件

```
{
  "mcpServers": {
    "qmd": {
      "command": "qmd",
      "args": ["mcp"]
    }
  }
}
```

1. **使用**

在文件夹中启动claude code,在新的文件夹中进行三步即可,让AI帮你解决

```
❯ 在一个新的文件夹里面需要吗

⏺ 需要。在新文件夹里要三步：

  # 1. 添加集合
  qmd collection add /path/to/新文件夹 --name 集合名

  # 2. 建立文本索引
  qmd update

  # 3. 生成向量嵌入
  qmd embed

  或者你也可以让我来做，告诉我文件夹路径和想要的集合名就行。
```

1. **后台守护模式**

```
# 启动守护进程，保持模型加载状态
qmd daemon start

# 搜索（速度更快，无需重复加载模型）
qmd query "认证流程" --daemon

# 停止守护进程
qmd daemon stop
```

**qmd会从hugging face下载模型，可以将镜像源更改，方便国内的下载**

```
# 临时设置镜像环境变量（仅在当前终端窗口生效）
export HF_ENDPOINT=https://hf-mirror.com

# 建议同时写入配置文件，避免每次重启终端都要重新设置
echo 'export HF_ENDPOINT=https://hf-mirror.com' >> ~/.bashrc
source ~/.bashrc
```

如果有显卡，可以使用`GGML_CUDA=1 qmd pull`强制使用显卡

# LLM-Wiki数据库搭建(五)--Obsidian Second Brain

## 6. obsidian-second-brain 使用

这个项目本质上是一个 “AI 驱动的 Obsidian 第二大脑操作系统”，而不是普通的 Obsidian 插件。它把 Obsidian Valut(Markdown 笔记库)变成一个能被 AI 持续维护、整理、研究和更新的知识库。

- ChatGPT / Claude 每次对话结束就失忆
- Obsidian 里的笔记越积越多，却没人帮你整理
- 大多数知识库只是不断追加内容（append-only），最终变成信息垃圾场

> Knowledge Base 不应该只是存储信息，而应该持续进化

**核心理念：OKM（Open Knowledge Metabolism）**

| 类型     | 含义           |
| :------- | :------------- |
| Timeless | 永久事实       |
| Dated    | 带时间戳的事实 |
| Pointer  | 指向来源       |



### 6.1 obsidian-second-brain 能做什么

目前已经有约45个命令

- AI研究助手
- 自动知识整合
- 定时Agent
- 思维工具
- 多平台支持

| 维度             | Karpathy 的 LLM Wiki                 | Obsidian Second Brain                                        |
| :--------------- | :----------------------------------- | :----------------------------------------------------------- |
| **核心理念**     | 用 LLM 帮你维护 Wiki                 | 构建一个能够自我维护的知识库                                 |
| **处理新资料**   | 新来源通常生成新页面，并建立交叉引用 | 新来源优先更新已有页面，人物信息更新、观点修订、过时事实替换 |
| **处理矛盾信息** | 标记冲突，由用户手动解决             | 通过 `/obsidian-reconcile` 自动分析并协调矛盾                |
| **发现知识模式** | 需要用户主动提问或探索               | 通过 `/obsidian-synthesize` 主动发现潜在模式，并自动生成综合分析页面 |
| **运行方式**     | 按需执行，用户主动触发               | 内置 4 个定时 Agent 持续运行                                 |
| **自动化能力**   | 基本依赖用户操作                     | 夜间总结、周度回顾、矛盾扫描、知识库健康检查自动执行         |
| **知识库演化**   | 以“新增内容”为主                     | 以“持续重写与演化”为主                                       |
| **笔记组织方式** | 偏传统 Wiki 结构                     | 偏知识代谢（Knowledge Metabolism）结构                       |
| **笔记格式**     | 面向人类阅读的 Wiki 页面             | AI 优先设计：包含 `## For future Claude` 预处理信息和专门的 Frontmatter，优化 LLM 检索与推理 |
| **知识更新机制** | 历史内容保留，容易积累过时信息       | 旧知识持续被修订，尽量保持当前状态                           |
| **用户角色**     | 用户负责维护知识库，LLM 提供辅助     | AI 与 Agent 持续维护知识库，用户负责监督与决策               |
| **最终形态**     | 一个由 LLM 协助维护的 Wiki           | 一个能够自我进化、自我整理、自我修正的第二大脑               |

**实际应用**:

- 在会议之后,使用`obsidian-save`命令,claude可以自动提取出每一个决定、人物、任务和想法，并将它们分别保存到相应的笔记中。你什么都不用做。
- 录音总结: `/obsidian-ingest meeting.m4a`,claude能够使用 Whisper 进行转录，识别说话人，提取每一项承诺和行动项，并将其分发到实体页面、任务板和每日笔记中。
- 截图,白板,video的内容也能够分析
- 在做出重大决定之前：`/obsidian-challenge` Claude 会搜索你的资料库，找出你过去在同一主题上的失败案例和推翻的决定。他会用你自己的话来反驳你。你的资料库会让你承担责任
- 想了解全局概览？运行 `/obsidian-visualize` 命令，Claude 会生成整个知识库的可视化画布。核心节点居中显示，按类型进行颜色编码，孤立节点高亮显示。在 Obsidian 中打开它，即可查看知识库的整体结构。
- 新的一天从 `/obsidian-daily` 开始。Claude 会将您的日历事件、逾期任务和夜间更改同步到今天的笔记中。让您的早晨从掌握信息开始
- 做研究的时候你输入一个研究主题，系统调用 Perplexity 的 Sonar Pro（或 Sonar Deep Research）去做类似“研究助理”的工作，然后把生成的研究报告自动保存进 Obsidian 知识库。

> 总体来说这个项目更是打包好一堆skill的知识库管理,所以称为second-brain

### 6.2 obsidian-second-brain 命令分级

| 层级                                       | 功能                    | 作用                                                         |
| :----------------------------------------- | :---------------------- | :----------------------------------------------------------- |
| **第一层：操作层（Operations）**           | 28 个命令               | 管理知识库、创建笔记、更新页面、整理任务，让 Claude 记住你的所有信息 |
| **第二层：思维工具层（Thinking Tools）**   | 8 个命令                | 作为思考伙伴，帮助分析问题、寻找漏洞、提出反方观点、进行决策推演 |
| **第三层：上下文引擎（Context Engine）**   | 1 个命令                | 建立个人背景模型，让 Claude 理解你的身份、目标、偏好和长期项目 |
| **第四层：研究工具层（Research Toolkit）** | 7 个命令                | 主动搜索和整合外部知识，包括 Web、X、YouTube、论文等资源     |
| **Always On：持续运行层**                  | 后台 Agent + 定时 Agent | 自动维护知识库、发现知识关联、生成总结、提醒保存重要信息     |

1. **操作层**

| 命令                          | 功能说明                                                     |
| :---------------------------- | :----------------------------------------------------------- |
| `/obsidian-save`              | 保存当前对话中的所有重要信息，包括决策、任务、人物、想法等，并写入知识库 |
| `/obsidian-ingest`            | 导入 URL、PDF、音频文件或截图；知识库会自动重写和更新，每个来源可能影响 5–15 个已有页面 |
| `/obsidian-synthesize`        | 自动发现多个来源之间的潜在模式，并生成综合分析页面           |
| `/obsidian-reconcile`         | 查找知识库中的矛盾信息并自动协调解决，让知识库维护自身“事实一致性” |
| `/obsidian-export`            | 导出干净的 JSON 或 Markdown 快照，可被任何 AI 工具读取       |
| `/obsidian-daily`             | 创建或更新当天的 Daily Note（日记/每日记录）                 |
| `/obsidian-calendar <mode>`   | 日历管理命令，支持 4 种模式：agenda（查看日程快照）、reconcile（发现未安排的承诺）、meeting（创建会议事件）、schedule（从任务或独立事件创建/移动日程） |
| `/obsidian-recurring`         | 管理周期性任务或长期责任，记录执行频率并自动计算下一次截止时间 |
| `/obsidian-log`               | 记录一次工作过程，并自动关联到相关项目、任务和知识页面       |
| `/obsidian-task`              | 添加任务到对应任务看板，并设置优先级和截止日期               |
| `/obsidian-person`            | 创建或更新人物信息页面                                       |
| `/obsidian-capture`           | 快速捕获灵感、想法，实现零阻力记录                           |
| `/obsidian-catchup`           | 处理 Telegram Bot 收集的内容（语音、文字、图片、PDF、链接），整理并写入知识库 |
| `/obsidian-find`              | 智能搜索知识库，并结合上下文返回结果                         |
| `/obsidian-recap`             | 生成某一天、某一周或某一个月的总结                           |
| `/obsidian-review`            | 执行结构化周总结或月度复盘                                   |
| `/obsidian-board`             | 查看和更新 Kanban 任务看板                                   |
| `/obsidian-board-hygiene`     | 批量整理任务看板：发现过期任务、停滞任务，并一次性归档、重新安排或标记完成 |
| `/obsidian-project`           | 创建项目页面，并关联任务看板和 Daily Note                    |
| `/obsidian-projects`          | 实时生成项目状态，通过 Git 和本地文档自动推断项目上下文，无需额外配置 |
| `/obsidian-health`            | 知识库健康检查：发现矛盾、知识缺口、过期内容、孤立页面、新鲜度违规，以及关系图中的错误连接 |
| `/obsidian-retrieval-eval`    | 评估知识库搜索质量，包括 Recall@K、MRR，并提供具体失败案例和优化建议 |
| `/obsidian-decide [--formal]` | 记录决策并关联到对应项目；`--formal` 模式生成完整 ADR（架构决策记录），保存决策背景和原因 |
| `/obsidian-visualize`         | 生成第二大脑的可视化知识地图（Canvas）                       |
| `/obsidian-learn`             | 回顾知识库中的学习内容，删除过时知识，发现规律并提炼为长期规则 |
| `/obsidian-init`              | 初始化 AI 知识库环境，生成 `_CLAUDE.md`、`index.md`、`log.md` 等核心文件 |
| `/obsidian-architect`         | 扫描代码库，自动生成并维护软件架构文档（总体结构、模块、设计决策等），重新运行即可刷新 |
| `/create-command`             | 通过 AI 访谈流程创建新的自定义命令，无需手动编辑 Markdown 文件 |

1. **思维层工具**

   

| 命令                                 | 功能说明                                                     |
| :----------------------------------- | :----------------------------------------------------------- |
| `/obsidian-brainstorm [topic]`       | 针对某个主题进行多轮苏格拉底式访谈。AI 每次只问一个关键问题，逐步帮助你澄清想法，直到形成完整方案，并生成包含多个备选方案的设计文档。 |
| `/obsidian-challenge`                | 利用你知识库中的历史记录和观点，主动反驳当前想法，寻找漏洞、盲点和隐藏假设。 |
| `/obsidian-panel`                    | 召集一个“虚拟专家评审团”，从多个不同视角（技术、商业、用户、风险等）评估一个决策，并生成综合结论。 |
| `/obsidian-emerge`                   | 分析最近 30 天的笔记，发现你自己从未明确命名过的模式、趋势和潜在主题。 |
| `/obsidian-connect [A] [B]`          | 将两个看似无关的领域连接起来，寻找跨领域创新机会和新思路。   |
| `/vault-deep-synthesis [topic]`      | 深度分析知识库中某个主题的所有相关笔记，找出共识、矛盾、过时观点和知识缺口。 |
| `/obsidian-distill [note or source]` | 将长篇笔记、论文或资料压缩成关键观点，并保留每条观点对应的原始出处。 |
| `/idea-discovery`                    | 从想法、未解决问题和零散研究中，筛选出最值得继续探索的 3–5 个方向。 |
| `/obsidian-graduate`                 | 将一个零散想法升级为完整项目，包括目标、任务、里程碑和执行计划。 |

1. **上下文引擎**

| 命令              | 功能说明                                                     |
| :---------------- | :----------------------------------------------------------- |
| `/obsidian-world` | 加载你的个人世界模型（身份、项目、目标、关系、当前状态等）。支持 L0–L3 四级上下文预算，根据需要逐步加载更多背景信息，让 Claude 在开始工作前先理解“你是谁、在做什么、什么对你重要”。 |

1. **研究工具包**

> Obsidian主动获取外部知识

- xAI Grok(实时X/Twitter信息)
- Perplexity Sonar(网页研究)
- Youtube
- Gemini File Search(Notebook LLM)

| 命令                        | 功能说明                                                     |
| :-------------------------- | :----------------------------------------------------------- |
| `/x-read [url]`             | 深度分析一条 X（Twitter）帖子，包括原文、完整讨论串、摘要、关键观点、回复情绪分析和主要声音 |
| `/x-pulse [topic]`          | 扫描 X 平台上的热门讨论，提取趋势主题、关键人物、热门观点和内容灵感 |
| `/research [topic]`         | 网页研究。生成带引用的完整研究档案，包括总结、时间线、关键事实、争议观点和开放问题 |
| `/research-deep [topic]`    | 知识库优先的深度研究。先扫描你的 Vault，发现知识缺口，再自动补充外部资料并更新相关页面 |
| `/notebooklm [topic]`       | 类似 Google NotebookLM。上传知识库中最相关的 12 篇笔记，用 Gemini File Search 生成带引用的答案 |
| `/youtube [url] [--visual]` | 提取 YouTube 视频字幕、元数据和热门评论并生成摘要；`--visual` 额外分析视频画面内容 |
| `/podcast [url]`            | 从 Apple Podcasts 或 RSS 获取播客内容，转录后生成 AI 摘要    |

1. **Obsidian**第二大脑的底层

| 场景                                    | 系统行为                                                     | 结果                                 |
| :-------------------------------------- | :----------------------------------------------------------- | :----------------------------------- |
| **导入一个新来源（Ingest a source）**   | 自动重写已有页面，解决矛盾信息，整合新旧知识，并生成新的综合分析 | 知识库持续演化，而不是简单新增笔记   |
| **保存一次对话（Save a conversation）** | 自动提取人物、概念、决策、任务和想法，并分发到对应页面       | 对话内容被结构化沉淀到整个知识网络中 |
| **提出一个问题（Ask a question）**      | 遵循“双输出规则（Two-Output Rule）”：既回答问题，也同步更新知识库页面 | 每次提问都会让知识库变得更完善       |
| **事实发生变化（A fact changes）**      | 使用“双时间轴事实（Bi-temporal Facts）”记录：事实何时为真，以及知识库何时得知该事实 | 完整保留认知演化过程和审计记录       |
| **什么都不做（Do nothing）**            | 后台 Agent 和定时 Agent 持续运行                             | 自动整理、维护和优化知识库           |
| **等待一段时间（Wait a week）**         | 自动综合（Auto-Synthesis）分析跨来源信息，发现隐藏模式和关联 | 自动生成新的连接页面和洞察总结       |

背景了解清楚之后,才能正确的使用该项目搭建LLM-wiki.



# LLM-Wiki数据库搭建(六)--Osb安装

### 6.3 Obsidian-second-brain安装

> 一套代码库，七个构建版本。请在下方选择您需要的版本。所有版本中的 Vault 行为完全相同；只有安装路径和调度程序文件（`CLAUDE.md` / `AGENTS.md` / `GEMINI.md` / `.agents/skills/` / `.pi`/）有所不同

Obsidian-second-brain 在Claude Code, Codex CLI, Gemini CLI, Hermes, OpenCode, Pi都经过了生成真实目录结构,脚本路径正确, 文档可访问和工具的可执行



#### 6.3.1 前置要求

**前置要求**:

- Claude Code(或者OpenAI, Hermes, Gemini, Codex CLI, Pi等)
- git的安装
- uv（用于运行 Python 辅助工具，例如健康检查、研究工具包和 Vault 初始化）
- jq（用于安全修改 ~/.claude/settings.json）

> scripts/setup.sh 会使用 jq 自动编辑配置文件，如果系统没有安装 jq，安装脚本会直接退出

- Ollama（用于本地语义搜索）
- openai-whisper（首次导入音频时自动安装，同时会安装 PyTorch）

Ollama和openai- whisper都是可选安装

| 软件               | 是否必须              | 用途                         |
| :----------------- | :-------------------- | :--------------------------- |
| Claude Code        | ✅                     | AI Agent 运行环境            |
| Git                | ✅                     | 下载和更新项目               |
| uv                 | ✅                     | Python 包管理和脚本运行      |
| jq                 | ⚠️ 部分安装方式需要    | 修改 Claude 配置文件         |
| Ollama             | ❌                     | 本地向量搜索、本地 Embedding |
| Whisper            | ❌                     | 音频转文字                   |
| OpenAI API Key     | ❌                     | 核心功能不需要               |
| Perplexity API Key | ❌（部分研究功能可选） | 增强 Research 能力           |
| xAI API Key        | ❌（部分研究功能可选） | X/Twitter 实时研究           |

后续都是以Claude Code为基础进行操作的

#### 6.3.2 安装

1. **插件安装**

安装原生插件（推荐）,在任何 Claude Code 会话中,输入插件安装

```
/plugin marketplace add eugeniughelbur/obsidian-second-brain
/plugin install obsidian-second-brain@obsidian-second-brain
```

安装完成后,在claude code中询问是否安装成功即可

![Image](D:\Typora\Typora\Markdown_image\640.png)

- 全部 45 个命令（Commands）
- 技能手册（Skill Manual）
- 会话上下文 Hook（Session Context Hook）
- 可选后台 Agent(默认不启用，需要手动开启)
- Vault MCP Server

> Valut MCP 是关键,claude code能找到仓库的位置,全靠环境env告诉claude code库的位置,在`~/.claude/settings.json` 配置

```
{
  "env": {
    "OBSIDIAN_VAULT_PATH": "/Users/yourname/my-vault"
  }
}
```

做完上述之后,重启Claude Code,然后进入你的 Vault 目录，在 Claude Code 中执行：`/obsidian-second-brain:obsidian-init`即可进行初始化了,初始化主要是建立目录和文件夹架构



1. **命令行安装**

直接安装 Skill（技能包），而不是作为插件安装.主要是使用简短形式,或者用来开发修改skills,改完后直接可以使用

```
curl -fsSL https://raw.githubusercontent.com/eugeniughelbur/obsidian-second-brain/main/scripts/quick-install.sh | bash
```

或者使用一步步安装,从git仓库clone下来

```cmd
# 1. 克隆仓库
git clone https://github.com/eugeniughelbur/obsidian-second-brain ~/.claude/skills/obsidian-second-brain

# 2. 安装
bash ~/.claude/skills/obsidian-second-brain/install.sh

# 3. 初始化仓库
bash ~/.claude/skills/obsidian-second-brain/scripts/setup.sh "/path/to/your/vault"
```

1. **其他平台使用**

CodeX CLI, Gemini CLI,OpenCode, Google Antigravity (and any .agents/skills/ harness), Pi Coding Agent, Run on Hermes / open models等都有具体的安装方法,按照github 上的说明进行安装即可[https://github.com/eugeniughelbur/obsidian-second-brain]

> 还没有数据库？那就先创建一个现成的数据保险库（包含文件夹、模板、看板、仪表盘——开箱即用，无需任何额外设置）:

```
# 1. 切换仓库中的py文件
cd ~/.claude/skills/obsidian-second-brain

# 2. 使用uv运行脚本
uv run python scripts/bootstrap_vault.py --path ~/Documents/MyVault --name "Your Name"

# 3. 初始化仓库
bash scripts/setup.sh ~/Documents/MyVault
```

# LLM-Wiki数据库搭建(七)--初级使用

### 6.4 Obsidian-second-brain 实际使用

1. **创建文件夹**

不管在本地也好,云端也好,在使用Obsidian-second-brain之前,都需要先创建一个文件夹,用来存放你的笔记,这个文件夹就是你的Vault, 这里在坚果云中创建一个`Gold`的文件夹

1. **文件夹中预设文件子夹**

下面是常规的文件夹架构,如果不使用这么复杂的架构,仓库中也提供了很多预设的模板对应不同的需求

> 如果使用了plugin安装,仓库就无法克隆,很多python文件就没,需要手动去下载下来运行,这里为了方便skill管理,所以使用了plugin安装,选择了plugin,就得把github仓库克隆下来使用其中的python脚本



1. 把git仓库克隆到当前文件中 `git clone https://github.com/eugeniughelbur/obsidian-second-brain ./obsidian-second-brain`

1. 选择自己需要的架构,比如`executive`, `builder`, `creator`或者`researcher` 来初始化文件夹,这里选择`researcher`

```
uv run python obsidian-second-brain/scripts/bootstrap_vault.py --path ./ --name "Gold" --preset researcher
```

1. 初始化后形成了下面的文件夹

| 文件夹           | 类别     | 作用                                 | 内容举例                               |
| :--------------- | :------- | :----------------------------------- | :------------------------------------- |
| `Sources/`       | 📥 输入层 | 原始资料存放区，不加工，保存最初来源 | PDF论文、网页,音频、视频、网页         |
| `Reading Queue/` | 📥 输入层 | 待读材料队列，记录未来需要处理的资料 | “待读：Nature 2026 究”                 |
| `Daily/`         | 📥 输入层 | 每日活动记录，一天一篇，作为信息入口 | `2026-07-26.md`                        |
| `Literature/`    | 🧠 处理层 | 文献理解后的笔记，与原始论文分离     | “机制阅读笔记”                         |
| `Hypotheses/`    | 🧠 处理层 | 研究假设、想法、待验证的问题         | “假设炎症反应”                         |
| `Methodology/`   | 🧠 处理层 | 实验方法、分析流程、技术方案         | RNA-seq流程、单细胞分析Pipeline、WB    |
| `Synthesis/`     | 📤 输出层 | AI跨多个来源总结产生的知识体系       | “调控机制综述”                         |
| `Projects/`      | 📤 输出层 | 项目管理中心，连接任务、资料、结果   | “生物标志物项目”                       |
| `People/`        | 🗂 管理层 | 人物知识卡片                         | 作者、合作人员、专家、研究对象         |
| `Boards/`        | 🗂 管理层 | Kanban任务看板                       | `Research.md`、`Writing.md`            |
| `Bases/`         | 🗂 管理层 | Obsidian Bases数据库视图             | 文献数据库、项目数据库、任务表         |
| `Templates/`     | 🗂 管理层 | 新建笔记模板                         | 文献模板、项目模板、Daily模板（约8种） |
| `_trash/`        | 🗂 管理层 | 删除文件暂存区                       | 已删除笔记                             |

> 除了_CLAUDE.md是必须的,每个都可以进行修改,去掉多余的,补充自己需要的,把自己的想法构思好即可

如果是命令行安装的,就不需要这么复杂,找到`~/.claude/skills/obsidian-second-brain`中的脚本运行即可

1. **env添加到claude code**

把当前文件夹加入到claude code的环境变量中去,如果不加入claude code将无法找到命令执行的目录,比如你执行了`obsidian-save`,claude code就会去当前目录下保存

```
{
  "env": {
    "OBSIDIAN_VAULT_PATH": "/Users/yourname/my-vault"
  }
}
```

> 活用AI,这里在目录中启动`claude code`,然后告诉ai`gold文件夹是否加入了claude code中env`,如果之前有在用户层会提醒是否有冲突,有冲突就把env加入到当前文件夹中,处于优先级

1. **让AI帮你来优化文件夹内容**

这些模板文件夹都是预设的,可以根据每个习惯来进行调整,直接告诉AI 修改文件夹即可,或者直接告诉AI按照下面的架构来创建文件夹也可以,每个人有每个人的习惯,不需要固化思维

```
vault/
+-- _CLAUDE.md          # Operating manual
+-- index.md            # Page catalog (Claude reads FIRST)
+-- log.md              # Activity timeline
+-- SOUL.md             # Your identity
+-- CRITICAL_FACTS.md   # ~120 tokens, always loaded (timezone, manager, location)
+-- raw/                # IMMUTABLE source material
+-- wiki/               # Claude's workspace
|   +-- entities/       # People, companies, tools
|   +-- concepts/       # Ideas, frameworks, synthesis
|   +-- projects/       # Project notes
|   +-- daily/          # Daily notes
|   +-- logs/           # Work session logs
|   +-- reviews/        # Weekly/monthly reviews
|   +-- tasks/          # Task notes
|   +-- decisions/      # ADRs
+-- boards/             # Kanban boards
+-- templates/          # Note templates
```

1. **Research 套件API环境搭配**

- 如果使用`plugin`安装obsidian-second-brain,是无法自动生成配置文件的,需要手动创建文件夹,放置配置文件

```
# 1. 创建文件夹

mkdir -p ~/.config/obsidian-second-brain

# 2. 创建.env文件
touch ~/.config/obsidian-second-brain/.env

# 3. 给.env文件添加权限
chmod 600 ~/.config/obsidian-second-brain/.env
```

- 如果是使用clone安装的,运行`bash ~/.claude/skills/obsidian-second-brain/install.sh`文件,回答`y`也是同样的效果,产生配置文件

> 通常初始化后会给一个`.env.example`文件,把文件复制到上述的`.env`即可,修改其中的API key

```
> cat .env.example
# obsidian-second-brain - research toolkit credentials
# Copy this file to ~/.config/obsidian-second-brain/.env and fill in the values.
# That path is Mac-local - never committed, never synced. Set permissions 600.

# --- Vault location (required) ------------------------------
# Absolute path to your Obsidian vault root. Research notes save here.
OBSIDIAN_VAULT_PATH=

# --- xAI Grok -----------------------------------------------
# Powers /x-read and /x-pulse (live X reading + trend analysis)
# Get key: https://console.x.ai
XAI_API_KEY=

# --- Perplexity ---------------------------------------------
# Powers /research and /research-deep (web research with citations)
# Get key: https://perplexity.ai/settings/api
PERPLEXITY_API_KEY=

# --- Tavily (optional) --------------------------------------
# Extra web-search source for /research free mode - joins the key-less pool
# when set, skipped silently when empty. Free tier available.
# Get key: https://app.tavily.com
TAVILY_API_KEY=

# --- Brave Search (optional) --------------------------------
# Extra web-search source for /research free mode - joins the key-less pool
# when set, skipped silently when empty. Requires a card: plans start at
# $5/1,000 requests with $5 free credits monthly (as of 2026-07).
# Get key: https://api-dashboard.search.brave.com
BRAVE_API_KEY=

# --- Google Gemini ------------------------------------------
# Powers /notebooklm (vault-grounded synthesis via Gemini File Search).
# Get key (free tier available): https://aistudio.google.com/apikey
GEMINI_API_KEY=

# --- YouTube Data API v3 (optional) -------------------------
# Powers /youtube metadata + comments. Transcripts work without this key.
# Get key: https://console.cloud.google.com → enable YouTube Data API v3
YOUTUBE_API_KEY=

# --- Model defaults (override if desired) -------------------
# xAI endpoint: https://api.x.ai/v1/responses (Agent Tools API)
# grok-4 (non-reasoning) is the right default for /x-read /x-pulse /youtube - these are
# extract-and-format tasks where reasoning is wasted overhead (3-4x more output tokens).
# Switch to grok-4.20-reasoning per-call if you want deeper analysis.
GROK_MODEL=grok-4
PERPLEXITY_RESEARCH_MODEL=sonar-pro
PERPLEXITY_DEEP_MODEL=sonar-deep-research
# Default /notebooklm model. Free tier supports gemini-2.5-flash; gemini-2.5-pro requires paid billing.
NOTEBOOKLM_MODEL=gemini-2.5-flash

# --- Auto-open behavior -------------------------------------
# After every research save, Obsidian opens automatically at the note.
# Set to 0 to disable (e.g. when running batch saves or scheduled).
# RESEARCH_AUTOOPEN=0
```



| Key                  | Where                        | Required for                                                 | Cost                                                         |
| :------------------- | :--------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| `XAI_API_KEY`        | `console.x.ai`               | `/x-read`, `/x-pulse`, `/research-deep`、X Pulse、YouTube summary | Pay-per-use，约 `$0.05/call`                                 |
| `PERPLEXITY_API_KEY` | `perplexity.ai/settings/api` | `/research`、`/research-deep`                                | Pay-per-use，约 `$0.02-$0.50/call`                           |
| `GEMINI_API_KEY`     | `aistudio.google.com/apikey` | `/notebooklm`、YouTube summary（Grok fallback）、基于 Vault 的 Gemini File Search synthesis | 免费额度覆盖；付费约 `$0.004/call`（Flash），`$0.06/call`（Pro） |
| `YOUTUBE_API_KEY`    | `console.cloud.google.com`   | YouTube metadata + comments（可选；transcripts 无需 API Key） | 免费额度 `10k units/day`                                     |
| `OPENAI_API_KEY`     | `platform.openai.com`        | Podcast Whisper transcription（可选；未设置时 fallback 到 show-notes） | 约 `$0.006/min`                                              |

1. **启用后台Agent**

```
  {
    "env": {
      "OBSIDIAN_VAULT_PATH": "/Gold",
      "OBSIDIAN_BG_AGENT_ENABLED": "1"
    }
  }
```

启用前你要知道的事

- 它在每次压缩上下文（compact）后自动跑，无人值守、--dangerously-skip-permissions，把会话里值 得留的东西写进 vault；
- 只能用 Read/Write/Edit/Glob/Grep，没有 Bash、没有网络、没有 MCP；
- 摘要里若混进密钥/密码/财务隐私，只写一行指针到 Staging，原始 secret 不落盘；
- 想关掉：把 "1" 改成 "0" 或删掉这行即可。

1. **定时任务**

| Agent     | 时间       | 对应命令                                                     |
| :-------- | :--------- | :----------------------------------------------------------- |
| `morning` | 08:00      | `/obsidian-daily`（每日盘评 + 待办/逾期任务）                |
| `nightly` | 22:00      | `/obsidian-reconcile` → `/obsidian-synthesize` → `/obsidian-health`（收尾、综合、修复孤儿链接） |
| `weekly`  | 周五 18:00 | `/obsidian-recap`（周回顾）                                  |
| `health`  | 周日 21:00 | `/obsidian-health`（Vault 健康审计）                         |

不同的定时机制有不同的优缺点

| 机制                      | 原理                                             | 优点                                                         | 缺点                                                         | 适用场景                                           |
| :------------------------ | :----------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- | :------------------------------------------------- |
| 会话内 cron（CronCreate） | Claude Code 会话内部创建周期任务                 | 配置简单，无需系统权限                                       | 依赖 Claude Code 保持运行；空闲/关闭时无法执行；周期任务约 7 天自动过期 | 临时提醒、短周期实验任务                           |
| launchd（macOS 系统级）   | macOS 原生 LaunchAgent/LaunchDaemon 定时启动任务 | 真正系统级定时；Mac 开机即可运行；Claude Code 关闭也能执行；长期稳定 | 需要编写 plist + runner；每次任务都是独立 headless Claude 调用；消耗 API/token | 日常自动化、Obsidian Vault 维护、长期 Agent 工作流 |

*自己可以设定架构*

| Agent   | 推荐机制 | 原因                                               |
| :------ | :------- | :------------------------------------------------- |
| morning | launchd  | 08:00 自动生成每日盘评，不依赖人工打开 Claude Code |
| nightly | launchd  | 22:00 自动执行完整 Vault 整理流程，属于核心自动化  |
| weekly  | launchd  | 固定周期回顾任务，适合无人值守                     |
| health  | launchd  | Vault 健康检查无需人工参与                         |

# LLM-Wiki数据库搭建(八)--高级使用

### 6.5 Obsidian-second-brain 高级使用

> 当上述设置完成后,即可开始完全使用obsidian-second-brain相关skills, 定时任务和搜索API不是必须的

- valut path是必须设置正确的
- obsidian-second-brain 安装是必须的,plugin或者命令行安装
- 文件夹创建是必须的

#### 6.5.1. **运行`obsidian-init`**

`obsidian-init`是用来初始化当前文件夹,首先是对`_CLAUDE.md`文档的初始化,下面是`_CLAUDE.md`实例模板:

```
# Claude Operating Manual - Gold's 黄金市场分析 Vault

> 在此 vault 做任何事之前先读此文件。
> 这是 Claude 在此处如何操作的唯一权威。

---

## AI-First Vault 规则（第 0 节 · 最先读，适用于每条笔记）

本 vault 为**未来的 Claude** 检索与推理而建，非供人逐篇阅读。主人很少直接打开笔记，而是调用 Claude 跨年份积累的知识做检索、综合、连点。**Claude 写入本 vault 的每条笔记必须遵守：**

1. **自包含：** 单条笔记须能独立解释自己；future-Claude 可能仅凭搜索拉到这一条，不能依赖反链补全语境。
2. **"For future Claude" 前言：** 每条知识笔记以 2-3 句摘要开头，10 秒判断相关性。
3. **富且一致的 frontmatter：** `type` / `date` / `tags` / `ai-first: true` 等可过滤元数据。
4. **每条外部事实带时间戳：** 如"央行 6 月购金约 74 吨（as of 2026-06, WGC）"，而非裸陈述。
5. **来源逐字保留：** 外部声明附原文 URL，便于多年后复核。
6. **强制双链：** 引用任何标的 / 项目 / 概念 / 数据源都用 `[[wikilinks]]`。
7. **置信度：** 标 `stated | high | medium | speculation`。

**例外（免前言 / 免富 frontmatter）：** root 操作文件（`_CLAUDE.md`、`Home.md`、`index.md`、`log.md`）、`Logs/YYYY-MM-DD.md`、board 文件、`raw/` 原始捕获。完整规范见 skill 的 `references/ai-first-rules.md`。本规则适用于所有 `/obsidian-*`、`/research*` 命令、后台代理，及任何直接写入。

---

## 行动前核对实时状态（第 0.5 节）

下任何市场判断前，先读**实时数据**，绝不从训练记忆推断行情、利率、日期；这些是会变的快变量，记忆里的值几乎必然过时：

- 报价位、收益率、ETF 吨位、COT 持仓、隐含概率 → 取实时值并附 `as of` 时间戳
- 经济数据公布 → 核对实际发布时间与实际值，不要凭印象
- 引用研报 / 新闻 → 附原文 URL 与日期，逐字保留来源

这是一条通用操作原则，写入此节让每个在此 vault 的 Claude 会话默认继承。

---

## Vault 身份

- **主人:** Gold
- **用途:** 黄金（XAU）市场深度分析
- **分析框架:** 宏观 / 技术 / 持仓 / 情绪 四象限（见 [[Frameworks/分析框架总览]]）

---

## 文件夹地图

| 文件夹 | 用途 |
|---|---|
| `Daily/` | 每日盘评。命名 `YYYY-MM-DD.md` |
| `Reports/` | 周报 / 月报 / 季报等定期报告 |
| `Data/` | 价格数据、图表截图、CSV 等原始数据 |
| `Sources/` | 研报、新闻、文章等原始材料（待读用 `status` 字段，聚合在 `_待读队列.md`） |
| `Views/` | 方向性观点 / 交易思路 / 跨来源综合推理（可检验判断） |
| `Frameworks/` | 分析框架与方法（宏观/技术/持仓/情绪） |
| `Projects/` | 深度专题（如"央行购金"、"实际利率与金价"） |
| `Watchlist/` | 跟踪标的 / 指标（每项一页，聚合在 Watchlist.base） |
| `Boards/` | 看板（`Research.md`） |
| `Bases/` | Obsidian Bases 数据库视图 |
| `Templates/` | 笔记模板 |
| `Archive/` | 过期报告 / 失效观点归档 |
| `_trash/` | 回收站（Obsidian 默认） |

---

## 关键文件

- **仪表盘:** `Home.md`
- **研究看板:** `Boards/Research.md`
- **分析框架:** `Frameworks/分析框架总览.md`

---

## 自动保存规则

Claude 应**无需询问**自动保存以下内容：
- 当日行情观察、关键数据、新闻驱动 → 当日 `Daily/` 盘评
- 新的研报 / 新闻 / 文章 → `Sources/`（新建时 `status: unread`，读完改 `read`）
- 新的方向性观点 / 交易思路 → `Views/`（含触发条件、目标止损、反证）
- 新的跟踪标的 / 指标 → `Watchlist/`（每项一页）
- 决定开始一个深度专题 → `Projects/` + 看板"分析中"
- 已完成的分析报告 → `Reports/`；跨来源综合推理随对应观点存入 `Views/`
- 任务项 → 看板 + Task 类型笔记

Claude 应**先问再保存**：
- 删除或归档现有笔记
- 移动笔记到 `Archive/`
- 任何涉及真实交易决策（入场/出场/仓位大小）的最终建议——先呈现，由人确认

---

## 命名规范

- 每日盘评: `YYYY-MM-DD.md`
- 周报/月报: `YYYY-MM-DD 周报.md` / `YYYY-MM 月报.md`
- 观点: 描述性标题（如 `实际利率转负前看多.md`）
- 跟踪标的: 资产名（如 `美元指数 DXY.md`、`SPDR黄金ETF GLD.md`）
- 归档前缀: `_archived_`

---

## 看板约定

优先级: 🔴 关键 · 🟡 重要 · 🟢 低

活动项：
```

- [ ] 🔴 **标题** · @{YYYY-MM-DD} 描述。 [[相关专题]] [[相关观点]]

```
完成项：
```

- [x] 🔴 **标题** ✅ Date

```
---

## 传播规则

| 事件 | 同时更新 |
|---|---|
| 新专题 | 看板（待跟踪→分析中）+ 当日盘评 |
| 新观点 | Views/ + 当日盘评 |
| 观点被证实/证伪 | 该 View 状态（含综合推理）+ 当日盘评 |
| 关键数据出炉 | 当日盘评 + 相关 Watchlist 标的页 |
| 周期报告完成 | Reports/ + 看板→已完成 |

---

*由 obsidian-second-brain bootstrap 生成，2026-07-26 为黄金市场分析重构。*
*重新生成：让 Claude "更新 _CLAUDE.md"*
```

**_CLAUDE.md 的作用可以从机制和内容两层看**:

1. *机制层：它是 Claude 进入这个 vault 的「开机指令」*

- 自动加载：每次新会话启动，load_vault_context hook 会把 _CLAUDE.md 自动注入 Claude的上下文一次。所以你不用每次提醒规则，Claude 默认就按它行事；Claude 也不需要在每条命令前重新读它

- 为什么带下划线 `_`：① 在 Obsidian 文件列表里排最前，一眼可见；② 标记为`root操作文件`，因此享受例外——它本身不需要像普通知识笔那样写`For future Claude 前言`或富frontmatter,就想python中的私有属性一样

  

- 它是 _CLAUDE.md，不是标准的 CLAUDE.md：标准 Claude Code 自动读的是无下划线的 CLAUDE.md；这里靠hook 显式加载，是 obsidian-second-brain 自己的约定

1. *内容层:它规定了 Claude 在此 vault 怎么干活*

| 优先级 | 章节                       | 作用                                                         |
| :----- | :------------------------- | :----------------------------------------------------------- |
| 1      | §0 AI-First 规则（最先读） | 定义本 Vault 为「未来的 Claude」而建；规定每条笔记必须自包含、带前言、富 frontmatter；外部事实必须标注 `as of`；保留原文 URL；强制使用 `[[双链]]`；标注意见/分析置信度；并列出规则例外。 |
| 2      | §0.5 实时数据核对          | 在进行任何市场判断前，必须优先获取实时行情、利率、宏观数据等信息；禁止依赖训练记忆推断快速变化变量。 |
| 3      | Vault 身份                 | 定义 Vault 的核心定位：主人为 Gold；主要用途为黄金分析；采用四象限分析框架：宏观（Macro）、技术（Technical）、持仓（Positioning）、情绪（Sentiment）。 |
| 4      | 文件夹地图                 | 定义 Vault 的目录结构及用途，包括 11 个核心文件夹，例如 `Daily/`、`Sources/`、`Views/`、`Projects/` 等，明确各类信息的存放位置。 |
| 5      | 自动保存规则               | 定义 AI 自动记录与需要确认的内容：无需询问即可保存盘评、研报、市场观点等；涉及删除、归档、真实交易建议等操作时必须先获得确认。 |
| 6      | 命名规范                   | 规定文件命名方式、标签规范、日期格式以及知识分类标准，保证 Vault 内容长期可维护。 |
| 7      | 看板约定                   | 定义 Dashboard 展示结构，包括市场状态、宏观环境、黄金趋势、技术位置、持仓变化、市场情绪、行动计划等模块。 |
| 8      | 传播规则                   | 定义信息在 Vault 内的流转方式；当重要事件发生时，需要同步更新 Daily、Sources、Projects、Views 等相关位置，避免信息孤岛。 |

#### 6.5.2 Obsidian skills复合使用

直接询问AI,怎么在当前文件夹中使用obsidian-second-brain,AI会给系列提示使用

1. 基础设施

| 组件       | 位置                 | 作用                                                         |
| :--------- | :------------------- | :----------------------------------------------------------- |
| 操作手册   | `_CLAUDE.md`         | 会话启动时由 Hook 自动加载；作为 Claude 行为规范的唯一权威文件。 |
| 目录       | `index.md`           | 全库笔记索引；Claude 首先读取，用于快速定位知识内容。        |
| 仪表盘     | `Home.md`            | 快速导航入口；展示近期盘评、市场观点以及 Watchlist。         |
| 研究看板   | `Boards/Research.md` | 管理研究流程状态：👀 待跟踪 / 🔬 分析中 / ✍️ 撰写中 / ✅ 已完成。 |
| 分析框架   | `Frameworks/`        | 存放核心分析方法，包括四象限框架、WGC 估值模型、GRAM 归因体系。 |
| 模板       | `Templates/`         | 存放标准化模板，包括 Daily / Weekly / Project / View / Source / Instrument / Task。 |
| 数据库视图 | `Bases/*.base`       | 提供结构化数据库视图，包括 Daily、Projects、Watchlist 三类视图。 |
| 操作日志   | `Logs/YYYY-MM-DD.md` | 每日操作记录；一天一个文件，仅允许追加，不修改历史记录。     |

1. 命令速查

| 场景            | 命令                                             | 作用                                                 | 产出位置                               |
| :-------------- | :----------------------------------------------- | :--------------------------------------------------- | :------------------------------------- |
| 每日盘评        | `/obsidian-daily`                                | 生成 / 更新当日盘评                                  | `Daily/`                               |
| 快速捕获        | `/obsidian-capture`                              | 记录一条灵感、观察或临时想法                         | 按类型自动落位                         |
| 吃进研报 / 新闻 | `/obsidian-ingest`                               | 将外部素材结构化入库                                 | `Sources/(unread)`                     |
| 联网研究        | `/research`、`/research-deep`                    | 围绕主题进行检索，并形成结构化研究文档               | `Sources/`、`Reports/`                 |
| 跨源综合        | `/obsidian-synthesize`                           | 综合多篇 Sources，寻找矛盾、共识与知识缺口           | `Views/`、专题目录                     |
| 全库深度综合    | `/vault-deep-synthesis`                          | 进行季报级跨库梳理与综合分析                         | `Reports/`                             |
| 形成观点        | 手写 / `/obsidian-capture`                       | 创建观点记录，必须包含触发条件、目标、止损、反证条件 | `Views/`                               |
| 反证检验        | `/obsidian-challenge`                            | 攻击已有观点，降低确认偏误                           | 对应 View                              |
| 记录决策        | `/obsidian-decide`                               | 记录决策过程、依据及后续跟踪事项                     | `Views/`、`Task/`                      |
| 开新专题        | `/obsidian-project`                              | 创建新的深度研究专题                                 | `Projects/` + 看板状态更新为「分析中」 |
| 统览专题        | `/obsidian-projects`                             | 查看所有专题及当前状态                               | `Projects/`                            |
| 检索            | `/obsidian-find`                                 | 跨 Vault 查找笔记、数据与观点                        | —                                      |
| 连点            | `/obsidian-connect`                              | 发现相关内容并补充关联关系                           | `[[双链]]`                             |
| 健康检查        | `/obsidian-health`                               | 检查断链、frontmatter 缺失、长期未更新专题等问题     | —                                      |
| 阶段复盘        | `/obsidian-recap`、`/obsidian-catchup`           | 回顾阶段成果、补充遗漏跟进事项                       | `Reports/`、日志                       |
| 外部素材        | `/x-read`、`/youtube`、`/podcast`、`/notebooklm` | 将不同来源内容转换为结构化笔记                       | `Sources/`                             |

1. 日常黄金分析的典型工作流串联

| 工作流     | 串联命令                                                    | 最终产出                  |
| :--------- | :---------------------------------------------------------- | :------------------------ |
| 每日跟踪   | `/obsidian-daily`（有新闻时追加 `/obsidian-ingest`）        | 当日盘评                  |
| 研报深读   | `/obsidian-ingest` → `/obsidian-synthesize` → 落入 `Views/` | 可检验观点                |
| 开深度专题 | `/obsidian-project` → 多次 `/research` + 综合分析 → 撰写    | `Reports/` + 看板状态完成 |
| 季度复盘   | `/vault-deep-synthesis` + `/obsidian-recap`                 | `Reports/`                |

> **只有在实践中不停的摸索,才能搭建好属于自己的知识库;不断修正,不选学习,不断改进,让AI融入自己的学习中**,不要局限于skill的使用,有自己的一套流程才是入门,主要是脑子中对于知识的积累和知识树的搭建

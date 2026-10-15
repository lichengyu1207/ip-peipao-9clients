# AI+IP陪跑变现操盘手 · 9大核心客户陪跑与转化 Skill（开源框架）

一个把"客户陪跑"变成可重复执行系统的开源 Skill。不教理论，只做执行：装进你的本地 AI 工具（豆包工作 / 扣子 / Trae / TraeWork / WorkBuddy 等），它就能帮你管客户、发跟进、推付费。

## 它能干什么

1. **管客户**：9 个核心客户档案（背景、付费状态、分层、卡点、下一步动作）一屏看全。
2. **发跟进**：按客户状态生成 1 对 1 私信，每次只给一条，不追单。
3. **分层转化**：按漏斗推进——9.9 元体验群（新线索）→ 600 元陪跑（主力付费层）→ 软件/企业版（2999+，高价值）。
4. **跑 SOP**：每日跟进流程（最多跟 3 人）+ 每周漏斗复盘，输出周报。

## 目录结构

```
ip-peipao-9clients/
├── README.md                  # 本说明
├── 使用说明.md                # 买家加载指引（拿到后怎么装、怎么用）
├── SKILL.md                   # 技能本体（客户档案为脱敏模板，替换成你的真实客户即可）
└── ip-peipao-9clients.zip     # 一键导入包（SKILL.md 位于压缩包根目录，供各平台上传承用）
```

## 支持平台与安装方法

> SKILL.md 是通用的开放技能格式（Anthropic Skills 标准），**68+ 款 AI 工具可直接读取**（详见下方「兼容生态」）。
>
> 买家版完整图文加载步骤见 **[使用说明.md](使用说明.md)**。

### 豆包工作（Doubao Work）

1. 打开豆包工作客户端，点击左侧「插件·技能·伙伴」→「技能」。
2. 点击「新建技能」，把 SKILL.md 全文粘贴进技能正文，保存。
3. 之后在任务中输入 `/` 或点击「更多技能」，选择该技能即可调用。

也可以直接对豆包说："根据 https://github.com/lichengyu1207/ip-peipao-9clients 创建技能"。

### 扣子（Coze）

- **扣子编程**：对话框 → 技能 → 编程技能 → 创建技能 → 本地上传（选择 zip 技能包）→ 在「我的技能」中添加。
- **扣子对话**：输入 `@` 或点击 `+` → 技能 → 添加技能。
- 提示：自定义技能为单次生效，每次开启新任务需重新添加。

### Trae（IDE / TraeCode）

1. 设置 →「技能 / 规则与技能」→「创建」。
2. 上传 `SKILL.md` 或包含 `SKILL.md` 的 zip（自动解析技能名称、描述、指令），确认即可。
3. 进阶：全局技能可手动放入 `~/.trae-cn/skills/<技能名>/SKILL.md`；项目级放入 `.trae/skills/`。

### TraeWork（SOLO）

1. 左侧边栏打开「Marketplace」→「Skills」页签。
2. 上传 `ip-peipao-9clients.zip`（或 `.skill` 文件）。
3. 注意：TraeWork 不支持直接上传单个 `.md` 文件，必须是根目录含 `SKILL.md` 的 zip。

### WorkBuddy

1. 技能页面 →「+ 添加技能」→「上传技能」。
2. 导入本地技能包（zip 或目录），系统自动完成配置，无需额外操作。
3. 进阶：也可从 GitHub / Gitee 导入；或手动放入 `~/.workbuddy/skills/<技能名>/SKILL.md`。

### 兼容生态（同格式直接可用）

SKILL.md 是 Anthropic 发布的开放技能标准，**68+ 款 AI 工具可直接读取**，主流包括：

- **编程 / IDE 代理**：Claude Code、Claude.ai、Cursor、Windsurf、OpenAI Codex、Gemini CLI、GitHub Copilot、VS Code、Qodo、Amp、Roo Code、Goose、Continue、Cline、Aider、OpenCode、Manus AI
- **本地智能体**：OpenClaw（`openclaw skills install git:lichengyu1207/ip-peipao-9clients`，或克隆到 `~/.openclaw/skills/`）、WorkBuddy（兼容 OpenClaw 生态）

安装方式基本一致：把含 SKILL.md 的文件夹放进该工具的 skills 目录，或通过其导入入口上传 zip。

## 怎么用

1. 按上面任一平台导入 SKILL.md（或直接下载 zip 上传）。
2. 打开 SKILL.md，把"客户A～客户I"替换成你的真实客户信息。
3. 之后直接说"跟进客户X"或"今天跟进谁"，Agent 会按策略出私信和动作。
4. 客户有新进展（付款/交作业/断联），告诉 Agent，它会同步更新档案。

## 配套

- 9.9 元体验群：拿开源 Skill 框架 + 基础用法答疑。
- 600 元陪跑：带你把整套流程跑通（定方向 → 搭工具 → 跑内容 → 跑变现）。
- 软件/企业版（2999+）：面向有团队、有规模的企业客户深度陪跑。

## 底线

- 不包安装、不包服务器、不包远程操作。
- 不免费咨询，深度问题用付费产品承接。
- 不逼单、不追单，只筛选愿意动的人。

## 版权与支持

© 2026 骇老师（AI+IP 陪跑变现操盘手）· https://github.com/lichengyu1207

- 本仓库是**开源框架**：可下载学习、可自由用于自己的业务。
- **禁止未授权转售 / 冒充原创 / 抹名分发**（详见 [LICENSE.md](LICENSE.md)）。
- 想转售？走 **C 转 B 授权**（详见 [PARTNER.md](PARTNER.md)）。
- 如果这套框架对你有帮助，**点一个 ⭐**——这是对作者最实在的支持，也是这套包持续更新的动力。

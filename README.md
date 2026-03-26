# 聘才猫 AI Skills

聘才猫（[pincaimao.com](https://www.pincaimao.com)）旗下 AI 智能体 skill 合集，可在 [OpenClaw](https://openclaw.ai) / [Claude Code](https://claude.ai/code) 等支持 ClawHub skill 的环境中使用。

所有 skill 均通过聘才猫开放 API 调用，需配置对应的 API Key 环境变量。

---

## 安装方式

```bash
# 安装单个 skill
clawhub install pincaimao-basic

# 安装全部 skill
clawhub install pincaimao-basic pincaimao-jd-assistants pincaimao-resume-diagnosis \
  pincaimao-resume-optimize pincaimao-career-planning-v2 pincaimao-interview-question \
  pincaimao-online-interview pincaimao-mock-interview pincaimao-interview-reports \
  pincaimao-labor-contracts
```

---

## Skill 列表

### 🏗️ 基础

| Skill | 说明 | 安装 |
|-------|------|------|
| [pincaimao-basic](https://clawhub.ai/orgs/pincaimao/pincaimao-basic) | 平台基础能力，所有其他 skill 的依赖，包含鉴权、文件上传、会话管理、SSE 解析模板等 | `clawhub install pincaimao-basic` |

> 其他所有 skill 都依赖 `pincaimao-basic`，请优先安装。

---

### 📝 招聘

| Skill | 说明 | 安装 |
|-------|------|------|
| [pincaimao-jd-assistants](https://clawhub.ai/orgs/pincaimao/pincaimao-jd-assistants) | JD 助手：根据职位描述生成招聘 JD，或根据职位名称生成结构化职位标签（技能/薪资/福利等维度） | `clawhub install pincaimao-jd-assistants` |

---

### 🎯 简历

| Skill | 说明 | 安装 |
|-------|------|------|
| [pincaimao-resume-diagnosis](https://clawhub.ai/orgs/pincaimao/pincaimao-resume-diagnosis) | 简历诊断：上传简历文件，结合职位描述分析候选人简历要点及岗位匹配程度 | `clawhub install pincaimao-resume-diagnosis` |
| [pincaimao-resume-optimize](https://clawhub.ai/orgs/pincaimao/pincaimao-resume-optimize) | 简历优化：根据目标职位智能分析岗位需求，自动优化或重写简历内容，提升与岗位的匹配度 | `clawhub install pincaimao-resume-optimize` |

---

### 🎭 面试

| Skill | 说明 | 安装 |
|-------|------|------|
| [pincaimao-interview-question](https://clawhub.ai/orgs/pincaimao/pincaimao-interview-question) | 面试出题大师：根据职位描述和候选人简历生成面试题目 | `clawhub install pincaimao-interview-question` |
| [pincaimao-online-interview](https://clawhub.ai/orgs/pincaimao/pincaimao-online-interview) | 在线面试（企业端）：多轮 AI 面试对话，支持文字/视频模式、自定义题目、报告回调 | `clawhub install pincaimao-online-interview` |
| [pincaimao-mock-interview](https://clawhub.ai/orgs/pincaimao/pincaimao-mock-interview) | 模拟面试（求职者端）：模拟真实面试场景，支持 HR/专业两种面试官角色、参考答案生成 | `clawhub install pincaimao-mock-interview` |
| [pincaimao-interview-reports](https://clawhub.ai/orgs/pincaimao/pincaimao-interview-reports) | 面试报告：根据职位描述和面试记录文件生成面试报告或辅导材料 | `clawhub install pincaimao-interview-reports` |

---

### 🚀 职业发展

| Skill | 说明 | 安装 |
|-------|------|------|
| [pincaimao-career-planning-v2](https://clawhub.ai/orgs/pincaimao/pincaimao-career-planning-v2) | 职业规划助手 V2：分析简历，针对「初入职场 / 转型建议 / 晋升路径」三种场景生成职业规划建议 | `clawhub install pincaimao-career-planning-v2` |

---

### ⚖️ 劳动权益

| Skill | 说明 | 安装 |
|-------|------|------|
| [pincaimao-labor-contracts](https://clawhub.ai/orgs/pincaimao/pincaimao-labor-contracts) | 劳动合同卫士：分析劳动合同文件或文本，生成合同解析报告和评估建议 | `clawhub install pincaimao-labor-contracts` |

---

## 快速上手

1. 在聘才猫平台创建 API Key：进入智能体页面 → 右上角「开发接入」→「API 导出」→「密钥管理」

2. 配置环境变量（以 JD 助手为例）：
   ```bash
   export PCM_JD_ASSISTANT_KEY=your_key_here
   ```

3. 安装并使用：
   ```bash
   clawhub install pincaimao-basic pincaimao-jd-assistants
   ```

4. 在对话中调用：
   > 帮我给「Java 高级工程师」这个职位生成一份招聘 JD，要求 5 年以上经验，薪资 25k-35k

---

## 相关链接

- 聘才猫官网：[pincaimao.com](https://www.pincaimao.com)
- ClawHub 主页：[clawhub.ai/orgs/pincaimao](https://clawhub.ai/orgs/pincaimao)
- 开发文档：[pincaimao.com](https://www.pincaimao.com)

ava 后端开发 · LLM 应用工程化 · 计算机科学与技术本科在读

你好，我是 Sakura。我写 Java 后端，最近一年专注做一件事：把 LLM 应用从 demo 做到能上生产——多智能体编排、RAG 检索质量、长会话上下文治理、流式输出、稳定性熔断，这些真问题一个一个解决掉。

🔭 主打项目
mockInterview — 多智能体模拟面试平台
上传简历与岗位 JD，AI 面试官多轮提问与追问、问满自动收尾；结束后报告线四智能体协作，产出逐题评分、点评与针对缺口的参考回答。

多智能体双形态：面试线确定性编排（时延敏感、零多余模型调用），报告线四智能体委派协作——评分、审稿质检回炉、参考回答、汇总
RAG 混合检索：自建 283 题 Markdown 题库按题号幂等入库 Milvus，稠密向量 + BM25 双路召回、RRF 融合；自建 45 条四形态评测集，分形态量化 hit@1 与 MRR
延迟优化：建会话冷创建 4.1s → 64ms（占位秒回 + 后台回填 + 首轮兜底）、出题 19~33s → 14.6~20.5s（ReAct 挂工具改预检索注入）
防作弊三振：无效作答严肃指出并换题，连续三次系统出面提前结束——模型打标、系统执法，纯提示词管不住的都上确定性闸门
工程化：端口-适配器分层（换模型引擎只动 infra 适配器）、168 个自动化测试、GitHub Actions 三 job CI、k6 压测（吞吐 +116%）、Resilience4j 熔断 + Prometheus/Grafana 可观测、Docker Compose 编排 MySQL/Redis/Milvus
技术栈：Java 21 · Spring Boot 3.4 · AgentScope-Java · MySQL · Redis · Milvus · Docker

🛠️ 技术栈
Java
Spring Boot
MySQL
Redis
Milvus
Docker
Linux
领域侧重：Agent 编排 · RAG 与检索评测 · 高并发缓存 · 消息队列 · 数据库调优

✍️ 写作
在 CSDN 记录 LLM 应用工程化的排查与优化过程（建会话延迟排查、隐藏思考流定位、检索评测集设计这类"真机抓 bug"向的内容）。

📫 联系
Email：3086044350@qq.com
正在寻找 Java 后端校招机会，欢迎交流


⭐ 觉得 mockInterview 有意思的话欢迎 star，也欢迎一起聊聊 Java 后端与 LLM 应用工程化。

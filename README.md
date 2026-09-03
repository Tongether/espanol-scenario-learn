# Espanol Vivo — 从真实场景开口说西班牙语

[![Demo](https://img.shields.io/badge/demo-online-brightgreen)](https://tongether.github.io/espanol-scenario-learn)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![No build](https://img.shields.io/badge/build-none%20required-blue)
![Single file](https://img.shields.io/badge/architecture-single%20HTML%20file-lightgrey)

一个面向中文母语者的西班牙语场景化学习工具。不用背单词书，直接走进 12 个真实场景，学即用。

**在线体验**：[https://Tongether.github.io/espanol-scenario-learn](https://Tongether.github.io/espanol-scenario-learn)

<!-- 录制 8-12 秒操作流后取消下面这行的注释：点场景 → 听发音 → 展开语法拆解 → 换词造句 -->
<!-- ![Espanol Vivo 演示](docs/screenshots/demo.gif) -->

---

**English**: A scenario-based Spanish learning tool built for Chinese speakers. Instead of starting from the
alphabet and grammar rules, it drops you straight into 12 real-life situations — airport check-in, ordering at a
restaurant, describing symptoms at a pharmacy — with 72+ dialogues you can tap to hear pronunciation.

- Colour-coded grammar breakdown for 70 key patterns, spelling out verb infinitive, person and tense for each chunk
- Spain vs Latin American Spanish: a dedicated page covering vosotros/ustedes, voseo, seseo, tense habits, a 30+ word comparison table and false-friend warnings such as `coger`
- 18 Spain-specific lines expand to show the Latin American wording, with audio
- Word-swap drills that generate and speak new sentences from a fixed pattern
- Letter and number pronunciation guides, a scenario-tagged mini dictionary, and a dialogue simulator
- No localStorage, no cookies, no tracking; installable to your home screen as a PWA
- One self-contained HTML file, zero dependencies, no build step — open it and it works

---

## 为什么做这个项目

市面上的西语学习工具要么太学术（从字母和语法规则开始），要么太碎片化（短视频刷完就忘）。对于即将去西班牙旅行、留学或工作的人来说，最迫切的需求是：**到了机场怎么值机？餐厅怎么点菜？生病了怎么描述症状？**

这个项目把学习场景拆成 12 个高频主题，每个主题包含 4-6 组真实对话，覆盖从社交寒暄到紧急求助的完整链路。

---

## 功能一览

| 功能 | 说明 |
|------|------|
| **场景对话** | 12 大主题，72+ 组对话，点击句子即可听发音 |
| **语法拆解** | 70 个高频句型的颜色编码词块分析，逐块说明动词原形、人称与时态。紫色=实词，粉色=语法块，蓝色=词尾变化，灰色=固定表达 |
| **地域差异** | 独立页面对比西班牙 vs 拉美西语：vosotros/ustedes、voseo、seseo 与阿根廷 ʃ 音、时态使用习惯、30+ 词对照表，以及 `coger` 这类用词雷区 |
| **句级地域对照** | 18 句西班牙特有说法可展开查看对应的拉美说法并朗读 |
| **换词造句** | 在固定句型中替换关键词，即时生成新句子并朗读 |
| **改词练习** | 每句对话附带情境化练习题，判分忽略重音与句末标点差异 |
| **字母发音** | 点击字母卡片听它在单词中的实际发音（不是字母名） |
| **数字发音** | 1-20、几十几规则、百位/千位、序数词及用法说明 |
| **西语小词典** | 按场景分类的高频词汇，支持模糊搜索 |
| **在线翻译** | 内置中文-西班牙语互译，支持语音朗读 |
| **对话示范** | 选择场景和对话，模拟真实聊天流程练习 |
| **安装到桌面** | 支持 PWA，手机可「添加到主屏幕」以独立窗口打开 |

> 不使用 localStorage、Cookie 或任何形式的本地存储，不记录学习行为。

<!-- 补 3 张静态截图后取消注释：场景对话页 / 语法拆解展开态 / 手机端窄屏 -->
<!--
| 场景对话 | 语法拆解 | 手机端 |
|---|---|---|
| ![](docs/screenshots/scenes.png) | ![](docs/screenshots/grammar.png) | ![](docs/screenshots/mobile.png) |
-->

---

## 12 个学习场景

1. 日常社交 — 打招呼、自我介绍、闲聊、告别
2. 餐厅点餐 — 找座位、点菜、叫服务员、结账
3. 购物买东西 — 问价、试穿、砍价、付款
4. 问路与交通 — 问路、地铁、打车、买票
5. 美食推荐 — 问哪里好吃、当地特色、评价食物
6. 机场 & 出入境 — 值机、行李超重、海关、登机口
7. 酒店住宿 — 入住、房型、客房服务、延迟退房
8. 银行 & 支付 — 换汇、开户、ATM、卡被冻结
9. 药店 & 就医 — 买药、描述症状、预约、取处方
10. 校园日常 — 报到、选课、借书、课堂提问
11. 影院 & 演出 & 景点 — 购票、博物馆、导览、音乐会
12. 紧急求助 — 丢东西、叫救护车、报警、迷路求助

---

## 技术栈

- **纯前端**：HTML + CSS + JavaScript，零框架依赖
- **单文件架构**：所有功能集成在一个 HTML 文件中，无需构建工具
- **Web Speech API**：浏览器原生西班牙语语音合成
- **MyMemory API**：免费翻译接口，支持中-西互译（每日额度有限）
- **零存储**：不使用 localStorage、Cookie 或任何本地存储，无状态
- **PWA**：可添加到手机主屏幕，以独立窗口启动
- **响应式布局**：适配手机、平板、桌面端

---

## 本地运行

```bash
# 直接双击打开 HTML 文件即可
# 或使用任意本地服务器
python -m http.server 8000
```

---

## 迭代记录

| 版本 | 更新内容 |
|------|----------|
| v1.0 | 基础场景对话、语法拆解、换词造句 |
| v1.1 | 新增数字发音模块、改词练习功能 |
| v1.2 | 新增 7 个场景（机场、酒店、银行、药店、校园、影院、紧急求助） |
| v1.3 | 词典增加搜索功能、内置在线翻译、角色扮演改名为对话示范 |
| v1.4 | 修复字母卡片双例词问题、翻译 API 升级为 LibreTranslate |
| v1.5 | **内容质量审核**：修正 21 处语法和表达错误，为西班牙特有词汇添加 🇪🇸 地域标注 |
| v1.6 | 修复对话示范死锁、语法拆解匹配失效等 11 项缺陷；翻译接口迁移至 MyMemory；补齐 SEO / 社交元信息与 MIT LICENSE |
| v1.7 | **语法拆解扩充至 70 个句型**；新增「地域差异」页与 18 句拉美说法对照；移除全部本地存储 |

---

## Roadmap

- [ ] 语法拆解继续扩充，目标覆盖全部有教学价值的句型
- [ ] 补充更多改词练习题
- [ ] 增加听力理解测试模式

---

## 开源协议

[MIT License](LICENSE)

---

**Made with curiosity for Spanish learners.**

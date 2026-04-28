---
# try also 'default' to start simple
# theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# some information about your slides (markdown enabled)
title: 个人履历
colorSchema: dark
paginate: true
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply UnoCSS classes to the current slide
highlighter: shiki
css: unocss
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: fade-out
# enable Comark Syntax: https://comark.dev/syntax/markdown
comark: true
# duration of the presentation
duration: 20min
exportFilename: slides_of_mine

---

<style scoped>
.slidev-layout {
    padding: 0px;
}

h1 {
  color: rgba(255, 255, 255, 0.95);
  text-shadow: 0px 0px 0.3em rgba(0, 0, 0, 0.381);
  box-shadow: rgba(0, 0, 0, 0.1) 0px 3px 8px;
}

img.main-background {
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  object-fit: cover;
}
</style>

<img class="main-background" src="/bg-pilot.png"/>
<h1 class="mt--70 backdrop-blur-xl p-9 text-shadow-3xl">
个人职业汇报
</h1>

---
hideInToc: true
---

# 目录

1. 基本信息

2. 工作简历

3. 重点项目

    - 网络边界安全建设 @ 理想汽车

    - 零信任安全网关 @ 快手

4. 职业规划

---
layout: section
---

# 一、基本信息

---
transition: fade-out
---


<div class="flex">

- **王骥腾**
- 1991年
- 当前：理想汽车 · 系统安全部 · 边界安全负责人
- 联系方式：imwjt@163.com / 131-4130-1934 

<div class="flex-1 text-center">
<img class="rounded-2xl w-70 m-auto" src="/avatar.jpg" />
</div>
</div>

---

## 教育背景

- **北京邮电大学** 计算机学院 · 软件安全中心 · 计算机技术专业硕士(保研) · _2013－2016_

- **北京邮电大学** 计算机学院 · 信息安全专业 · 全日制本科 · _2009－2013_

## Publication

- **王骥腾**, 徐国爱, 王子宁. 《一种面向工业控制系统的脆弱性拓扑分析技术》. VARA 2014. 

- 郭燕慧, **王骥腾**. 《基于行间距的文档水印的研究与性能分析》. VARA 2014. 

- Zhenbo Xu, Jian Zhang, Zhongxing Xu, **Jiteng Wang**, "Canalyze: A Static Bug-Finding Tool for C Programs", ISSTA 2014.

## 认证

- **CISP**（注册信息安全工程师），中国信息安全测评中心：CNITSEC2017CISE02995
- **PMP**（项目管理专家），PMI 机构

---
layout: section
---

# 二、工作经历

---
layout: center
---


|        |  **岗位**       | **主要工作**      |
| --------------------------------------------------- | --------------------------- |----------|
| 2022.02 — 至今    @ **理想汽车**                | 系统安全部 · 边界安全部门负责人  | 企业网络边界安全 |
| 2018.09 — 2022.02 @ **快手** | 信息安全部 · 高级研发工程师 | 企业级零信任网关 |
| 2015.10 — 2018.08 @ **中国民生银行**  | 总行信息科技部 ·  信息安全工程师 | 安全平台 & SDL 建设 |
| 2015.05 — 2015.09 @ **VMware** | HWU · 研发工程师实习 | vSwitch 自动化工具 |


---

## 个人优势



- 10 年企业安全建设经历

- 经历过 0 -> 1 企业安全建设(**快手** & **理想**) ，行动路径清晰

- 丰富 **安全研发** 和 **基础设施稳定性** 经验，深入理解生产效率与安全建设平衡

---
layout: section
---

# 三、重点项目经历

---
layout: center
---

# 项目 1：零信任安全网关 AccessProxy @ 快手

---

## 项目背景


- 传统网络安全方案中的 [~~内 网 默 认 安 全~~]{style="color:orange"} :inline-component{prop="value"} 理念失效

- 云基础设施（K8S 和容器化）成为主流，防火墙用于网络隔离的局限性凸显

- 移动办公兴起，单纯 VPN 内网模式越发笨重 

******
<br>

### 零信任概念

[零信任（Zero Trust）]{style="color:yellow"}是一种网络安全模型，其核心理念是“永不信任，始终验证”。

零信任假设所有访问都不可信，必须经过[持续不断]{style="color:yellow"}的身份验证、权限控制和监控来确保安全。

2014 年起，Google 开始在 _USENIX ;login:_ 杂志发表其 BeyondCorp 企业安全架构的落地细节，行业将其视为零信任模型的教科书级工程落地。


---

## 传统企业网络架构

<div class="flex justify-center items-center h-full">
  <img src="/perimeter_model.svg" class="w-[95vw] max-h-[85vh] object-contain" />
</div>

---

## AccessProxy 解决方案

<br>

1. 企业级反向代理：将所有向 IDC 内 HTTP 服务的访问收敛至 AccessProxy 网关

2. 全局安全策略执行点：托管员工访问服务的认证、授权，支持数据水印（流量修改）

3. 打通企业Single-Sign-On (SSO)、KIM，实现员工无感认证、多因子认证

4. 作为底层数据源：为数据安全、员工异常审计提供数据底座

---

## AccessProxy 解决方案

<div class="flex justify-center items-center h-full">
  <img src="/ztna.svg" class="w-[100vw] max-h-[100vh] object-contain" />
</div>

---

## 成果

1. **研发落地**：多因子认证 / 数据水印 / HTTP2 协议支持 / 流量控制 / 动态服务发现 

2. **安全效果**：流量收口 / 认证全量覆盖 / 统一策略执行点 / 风险审计数据源

3. **办公效率**：3W+ 员工的稳定办公生产力保证 / 0 到 1 高可用架构搭建 / 容灾方案落地 

4. **企业级活动保障（0 故障）**：

    - 70 周年国庆阅兵直播保障

    - [_2020 年央视春晚红包保障_]{style="color:yellow"} :inline-component{prop="value"}  (冠名赞助春晚)

    - 2021 年春晚直播保障

    - 周杰伦内地首场直播保障

---
layout: center 
---

# 项目 2：网络边界安全建设 @ 理想汽车

---
layout: center
---

## 项目背景


<style scoped>
.slidev-layout table th {
    background-color: #1e293b;
    color: #f1f5f9;
    font-weight: 700;
    font-size: 1.2rem;
    padding: 0.6rem 1rem;
    border-bottom: 2px solid #22d3ee;
  }

  .slidev-layout table td {
    padding: 0.5rem 1rem;
    border-bottom: 1px solid #1e293b;
  }
</style>

<br>
<br>

| 关键问题 |  |
|------|---------|
| **云网关缺失** | 存量 WAF（Web Application Firewall） 补位，同时充当网关和防护组件 |
| **防护薄弱，风险严峻** | WAF 与业界方案脱节，黑客攻击频发；因频繁扫描，官网等主站宕机 | 
| **核心协议未覆盖** | 核心产品（车云通信链路）缺少防护 |
| **办公安全防护缺失** | 缺失网络边界防护，数据泄漏风险加剧 |


---
layout: center
---

## 项目背景

<div class="flex justify-center items-center h-full">
  <img src="/waf_legacy.svg" class="w-[100vw] max-h-[100vh] object-contain" />
</div>

---
layout: center
---

## 成果

<style scoped>
.slidev-layout table th {
    background-color: #1e293b;
    color: #f1f5f9;
    font-weight: 700;
    font-size: 1.2rem;
    padding: 0.6rem 1rem;
    border-bottom: 2px solid #22d3ee;
  }

  .slidev-layout table td {
    padding: 0.5rem 1rem;
    border-bottom: 1px solid #1e293b;
  }
</style>

<br>

- **重构流量接入架构**：推动接入层与防护组件拆分，推动新架构平稳切换、全量覆盖

- **升级防护能力**：工业级检测引擎 ModSecurity · 攻击扫描对抗自动化 · JA4 客户端指纹 

- **支持车云私有协议**：落地车云应用防火墙 _VCAF_

- **办公网络管控**：零信任网关落地

<br>

#### **其他**

- **运营提效**：实现 LLM 运营助手，识别海量流量中的误报，人效大幅提升

- **数据安全基础设施**： 全流量记录 + 关键数据采样，构建离线风险分析底座

- **能力验证**： 2025 年"国家 HW 演练"中负责边界防护，负责领域 0 入侵 0 失分

---

## 成果

<div class="flex justify-center items-center h-full">
  <img src="/waf2.svg" class="w-[100vw] max-h-[100vh] object-contain" />
</div>

---
layout: section
---

# 四、职业规划

<br>

---
layout: center
---

## 规划：建设研究院纵深防护体系                                                                                                                                                                                                                              
<br>

<div class="flex justify-center items-center h-full">
  <img src="/did_layers.webp" class="w-[80vw] max-h-[80vh] object-contain" />
</div>

---

## 行动事项

<br>

- **网络安全**：网络区域划分隔离 / 流量收口 / 零信任 / WAF / Anti-DDoS 流量清洗

- **主机安全**：主机入侵检测系统 HIDS / K8S 容器安全 CWPP

- **办公内网安全**：设备准入 / BYOD 设备管理 / 反病毒 / 员工安全培训
```
BYOD: Bring-Your-Own-Devices，指个人设备用于企业办公的场景
```

- **态势感知与应急响应**：安全信息事件管理SIEM / 安全运营中心SOC

- **数据安全**：终端 DLP / NDLP / git 代码保护

- **……** （根据研究院实际情况评估优先级，顺序落地）


---

## 初步计划

<br>

|         |    短期   |    中期 (1 - 2年)    |    长期 (3 - 5年)    |
| -------- | --------------------- | ----------------- | -------- |
|**网络安全**|网络分区隔离 + 网络收口| WAF / 零信任网关 | 面向科研 / 产研场景的服务级微隔离 |
|**反入侵**| NIDS部署 | HIDS 开发与部署 | AI 驱动的自动化安全运营|
|**办公安全**| 安全培训 | 网络准入 / 终端反病毒 |  BYOD 管理 / 全员零信任访问 |
|**数据安全**| 终端 DLP 调研 | DLP 推广 / git 仓库分级、保护 |  数据库保护 / 数据分级分类 |
| …… |


---
layout: end
---

# 感谢观看

Q&A


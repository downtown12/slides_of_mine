---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: resume
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable Comark Syntax: https://comark.dev/syntax/markdown
comark: true
# duration of the presentation
duration: 20min
layout: center
---

# Self Presentation

---
layout: center
---

# 基本信息

---
transition: fade-out
layout: two-cols
layoutClass: gap-16
---

# 王骥腾

■ imwjt@163.com 

· (+86) 131-4130-1934 

· https://github.com/downtown12 

· 1991年 中共党员

· 北邮本硕 -> 银行业 -> 快手 -> 理想汽车

::right::

![avatar](./testavt.png)

---

## 教育背景

- **北京邮电大学** 计算机学院 · 软件安全中心 · 计算机技术专业硕士（保研/全日制）2013－2016

- **北京邮电大学** 计算机学院 · 信息安全专业学士（全日制本科）2009－2013

## Publication

- Zhenbo Xu, Jian Zhang, Zhongxing Xu, **Jiteng Wang**, "Canalyze: A Static Bug-Finding Tool for C Programs", ISSTA 2014.

- **王骥腾**, 徐国爱, 王子宁. 《一种面向工业控制系统的脆弱性拓扑分析技术》. VARA 2014. 

- 郭燕慧, **王骥腾**. 《基于行间距的文档水印的研究与性能分析》. VARA 2014. 

---

# 认证

- **CISP**（注册信息安全工程师），中国信息安全测评中心：CNITSEC2017CISE02995
- **PMP**（项目管理专家），PMI 机构

# 专业技能

- **程序语言**：熟练 Python、Lua、SQL；熟悉 C、Shell、JavaScript；了解 Go
- **开发组件**：熟练使用 Grafana、Kafka、ELK、Clickhouse、Redis、MySQL
- **网络协议**：熟练 HTTP/1.X，熟悉 HTTP/2、TCP/IP、DNS
- **开发工具**：熟练掌握 Linux 平台的开发工具、调试、debug 技巧

---
layout: section
---

# 工作经历

---

# 理想汽车
**2022.02 — 至今** · 系统安全部 · 边界安全部门负责人

- 理想汽车企业边界安全保障和技术体系建设
- 边界静态防护到**零信任+动态威胁防护**的全量替换
- **0** 入侵事件，25年国家级演练 0 失分
- 6 人团队

---

# 快手科技
**2018.09 — 2022.02** · 信息安全部 · 高级研发工程师 / 内部讲师


- 企业级安全网关 AccessProxy 项目负责人
- 参考 Google BeyondCorp "零信任"方案：反向代理 + 认证/授权/审计
- 实现 3W+ 员工访问企业内部 1W+ 应用服务的唯一通道。员工无需 VPN 即可随处安全地访问企业应用
- 数万 QPS 下办公安全稳定

---

# 中国民生银行总行信息科技部 
2015.10 — 2018.08 · 安全规划中心 · 信息安全工程师

- 民生银行漏洞预警系统。
- Github 代码外泄巡检服务

---

# VMware, Inc
2015.05 - 2015.09 · HWU 测试研发工程师实习

- 负责 docstring2docx 系统开发，将虚拟交换机 vSwitch 项目代码中的函数注释自动转换为 docx 格式的富文本文档，提供给部门客户使用。使用有限自动机模型，基于 Python 开发。

---
layout: section
---

# 重点项目经历

---

# 边界安全建设 @ 理想汽车

## 背景

## 架构

## 成果

---

# 零信任安全网关 AccessProxy @ 快手

## 背景
1. 传统企业安全建设理念的打破
> -- 互联网无限危险，内网无限可信 --
2. 远程办公、移动办公兴起，VPN 连入内网模式变得笨重 

## 架构

- 一个企业级的反向代理
- 对企业服务访问认证、授权和流量审计的托管
- 打通企业Single-Sign-On (SSO)、KIM
- 与DNS、防火墙、VPN、UEBA等安全组件相互配合

## 成果

**主要成果**

1. **产品研发**：研发落地了包括但不限于以下核心功能：多因子认证、流量控制、服务发现、请求特征路由转发、HTTP/2 协议接入。
2. **2020 年央视春晚官方赞助红包保障、2021 年央视春晚现场保障**：负责 AccessProxy 和稳定性架构、容灾逃生方案、监控系统的设计落地以及现场 oncall。
3. **大型活动稳定性保障**：在国庆 70 周年阅兵、周杰伦内地首场直播等多次大型直播活动中，负责 AccessProxy 和企业 SSO 服务的稳定性保障，实现 0 异常和 0 故障。
4. **HTTP 流量镜像服务**：负责镜像用户的完整请求和响应，并异步发送至 Kafka 消息队列，供给其他安全业务团队。推广接入了数百个内部应用系统，基于 OpenResty 实现。

---
layout: section
---

# 职业规划

---

## 优势

- 丰富的甲方安全厂商从业经验
- 涵盖开发、规划、运营领域


## 匹配度

- 0 -> 1 安全建设经历和实践，匹配当前公司需求
- 能够亲自上手建设，丰富的稳定性经验

---
layout: section
---

Thanks!

---

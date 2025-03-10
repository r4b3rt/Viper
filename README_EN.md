<p align="center">
   <img width="200" src="https://cdn.nlark.com/yuque/0/2020/svg/159259/1590851265515-f865560b-ba50-4ca3-b2f6-5e8db3268da1.svg#align=left&display=inline&height=200&margin=%5Bobject%20Object%5D&name=logo.svg&originHeight=200&originWidth=200&size=1378&status=done&style=none&width=200">
</p>

English | [简体中文](./README.md)

- Viper is a graphical internet attack surface management & red team simulation platform.
- Viper modularizes and weaponizes the tactics and techniques commonly used in internal network penetration.
- Viper covers the common functions of red team simulations (anti-virus bypass, internal network tunnels, file management, command line, etc.).
- Viper red team simulation currently integrates more than 100 modules, covering all major tactics of MITRE ATT&CK.
- Viper has a built-in red team LLM agent that can use natural language to perform internal network information gathering/lateral movement/phishing email generation, etc.
- The goal of Viper is to help red team engineers improve attack efficiency, simplify operations, and lower technical barriers.
- Viper attack surface management supports collection and management functions for filing/domains/IPs/public account mini-programs/CDN/WAF/vulnerabilities, etc.
- Viper supports running native msfconsole in a browser and supports multi-person collaboration.

<br>

![image.png](https://cdn.nlark.com/yuque/0/2021/png/159259/1631688473804-d80f746b-e2fd-4d53-a44e-8bf8c4dc89d1.png?x-oss-process=image%2Fresize%2Cw_2250%2Climit_0)
<br>
<br>
<br>
![image.png](https://cdn.nlark.com/yuque/0/2021/png/159259/1631688521936-66b17009-3830-4925-941d-aad201252f90.png?x-oss-process=image%2Fresize%2Cw_2256%2Climit_0)
<br>
<br>
<br>
![image.png](https://cdn.nlark.com/yuque/0/2021/png/159259/1631688605817-27cf835d-fd4c-42cc-95a1-880ea5cf9102.png?x-oss-process=image%2Fresize%2Cw_2256%2Climit_0)
<br>
<br>
<br>
![image.png](https://cdn.nlark.com/yuque/0/2021/png/159259/1631688493291-48972160-0e2a-4757-a3a0-a466003d98f3.png?x-oss-process=image%2Fresize%2Cw_2256%2Climit_0)
<br>
<br>
<br>
![image.png](https://cdn.nlark.com/yuque/0/2021/png/159259/1631688640236-8f79ff40-e012-4fe8-89ce-cfcf2fd6627e.png?x-oss-process=image%2Fresize%2Cw_2256%2Climit_0)
<br>
<br>
<br>
![image.png](https://cdn.nlark.com/yuque/0/2021/png/159259/1631688660123-906ed19d-a6df-4632-8169-b6edf50c6ef7.png?x-oss-process=image%2Fresize%2Cw_2256%2Climit_0)
<br>

# Website

- [https://www.yuque.com/viper-en](https://www.yuque.com/viper-en?language=en-us)

# Installation manual

- [Installation manual](https://www.yuque.com/viper-en/inh85g/cvucxz?language=en-us)

# Updatelog

<details>
<summary><b>✨Click to expand</b></summary>

## v3.0.0 2024-12-09-10-50-06
### New Features
- screen_share function supports direct preview on the web end
- Added 'Filing', 'Favicon' and other features to attack surface management
- Automatically block login when Viper is brute-forced

## Optimizations
- Updated AI module prompts
- Switched attack surface management data storage from sqlite to elasticsearch
- Updated the startup sequence of backend services, added logs for reasons of startup failure
- Merged Metasploit-Framework version 6.4.40


## v2.3.5 2024-09-29-16-32-42
### New Features
- webcam_stream function supports direct preview on the web end

### Optimizations
- Supports entering a custom model name for `OPENAI`
- Improved error message when `OPENAI` is not configured
- Updated API for the 'Get Internet Exit IP' module to https://ipwho.is/
- Prompt updates for 'Email Generation/Sending Agent' and 'Platform Operation Agent', introducing CoT and Role Play

## v2.3.4 2024-09-04-16-59-30
### New Features
- Added 'Multi-user' feature, supporting multi-person collaboration

### Optimizations
- 'Smart Assistant' now supports output and display in Markdown format


## v2.3.3 2024-08-21-11-24-51

### Optimizations
- Updated some smart agent prompts
- 'Email Generation/Sending Agent' can now add and send attachments
- Reconstructed all smart agents using langgraph
- Automatic cleanup of ToolCall and Tool Message to reduce token usage

### Bugfixes
- Fixed https://github.com/FunnyWolf/Viper/issues/225

## v2.3.2 2024-08-05-15-27-29

### New Features

- Added 'SMTP Configuration' for sending emails
- 'Data Analysis Multi-role Agent' supports querying and analyzing session/handler related information
- 'Data Analysis Multi-role Agent' supports Meterpreter-related operations (camera/stream capture/keystroke logging/file viewing)
- Added 'Email Generation/Sending Agent', which can generate complete emails and send them based on user description

### Optimizations

- Adjusted some button UIs
- 'OpenAI' adds 'gpt-4o-mini' model
- Added heartbeat detection for service status checks in 'Penetration Service'
- Code for 'Internet Attack Surface Management' workers has been merged into the main branch

### Bugfixes

- Fixed interface jitter issues

## v2.3.1 2024-07-08-16-03-05

### New Features

- Introduced 'V-GPT', an AI-driven offensive intelligent agent framework
- Added 'Data Analysis Agent' and 'Data Analysis Multi-role Agent' modules
- Integrated 'OpenAI'

### Optimizations

- Adjusted parts of the 'Platform Settings' UI

### Bugfixes

- Fixed https://github.com/FunnyWolf/Viper/issues/217
- Fixed https://github.com/FunnyWolf/Viper/issues/218

## v2.3.0 2024-05-08-17-00-11

### Optimizations

- Adjusted the overall architecture of 'Internet Attack Surface'
- Enhanced 'Network Asset' search functionality
- Optimized data storage efficiency for 'Internet Attack Surface'
- Adapted to new API interfaces of Quake

### Bugfixes

- Fixed the issue where modules could not use newly established listeners
- Fixed the inability to use 'Anti-tracing'
- Fixed the timeout issue of creating new listeners when host performance is insufficient

## v2.2.1 2024-04-21-13-52-18

### New Features

- Added 'General Configuration' page, allowing configuration for 'Web Search Engine', 'wafw00f' related settings

### Optimizations

- Added wafw00f check to 'Service Status'
- Automatically redirects to login when accessing navigation pages without being logged in
- Nuclei now supports setting vulnerability levels and concurrency numbers
- Updated 360 Quake interface
- Optimized wafw00f performance (gevent)
- Improved frontend error messages when module errors occur
- Interpreter updated to Python 3.12 and pip dependencies updated to the latest versions
- Merged Metasploit-Framework version 6.4.6

### Bugfixes

- Fixed https://github.com/FunnyWolf/Viper/issues/207
- Fixed low probability encoding errors when generating C code


## v1.5.18 20220311
### Optimize
- After Viper restarts, it will no longer automatically load historical handler, but generate corresponding virtual handler and add the "backup" label to facilitate manual recovery
- Use jemalloc Ruby to optimize MSF memory use
- Merge Metasploit Framework version 6.1.34
### Bugfix
- Fix port occupation after reverse_https is closed
- The handler generated by to_handler is correctly displayedin WEBUI


## v1.5.17 20220305
### New features
- Add Android into `Payload And Handler`
### Optimize
- Merge Metasploit Framework version 6.1.33
### Bugfix
- Fix the problem that msfrpc generates a large number of 127.0.0.1 connect
- Repairing 'docker health check' cause a large number of 'TIME_WAIT' connect

## v1.5.16 20220226
### Optimize
- Optimize UI and adapt to macox
- Merge Metasploit Framework version 6.1.32
### Bugfix
- Fix `Fake exe file of Word document` exe cannot be cleaned up in some situations
- Fix the problem that `Python/Java/Android` payloads cannot online

## v1.5.15 20220213
### Optimize
- Optimize UI
- Delete session add secondary confirmation
- `communication channel` adapts to most payloads
- Merge Metasploit Framework version 6.1.30
### Bugfix
- Fix the MIUI crash problem of `mobile camera taking photos`


## v1.5.14 20220206
### New features
- Add three Android teaching demonstration modules (obtain target mobile phone SMS / call record / address book) (take photos with mobile phone camera) (record audio with mobile phone)
- The 'session channel' function is added to make multi-level intranet penetration more convenient [readme](https://www.yuque.com/vipersec/blog/gssfbg)
### Optimize
- Merge Metasploit Framework version 6.1.29

## v1.5.13 20220111

### New features
- Added zoomeye API interface
- Add `dnslog server` module

### Optimize
- Delete the "InternetScan" debug interface (the manual import function can completely replace this interface)
- Log4j payload echo java version, OS arch, OS version
- Optimize the pipeline logic of `InternetScan`, which will not affect the heartbeat data transmission at present
- Merge Metasploit Framework version 6.1.25

### Bugfix
- Fix the problem that the `VMware horizon log4j rce` timeout parameter does not take effect



## v1.5.12 20211231

### New features

- New passive scanning framework
- Added `VMware horizon log4j rce` InternetScan module
- Add `LDAP server` module to graphically manage ldapserver

### Optimize

- Log4j rce passive scanning function updated to passive scanning module
- Update the bypass WAF payload of log4j rce
- `Log4j CVE-2021-44228 Scan` add timeout parameter

## v1.5.10 20211216

### New Features

- New log4j passive scanning function
- Viper + crawlergo can be used in combination to automatically and actively scan log4j vulnerabilities

### Log4j passive scan

- Automatically replace the get request parameter with payload
- The auto replace post request parameter is payload
- The JSON value of auto replace post request is payload
- Auto replace skip password field
- Automatically add payload in headers (polling by Dictionary)
- The payload contains the original payload and the payload bypassing the WAF
- The payload contains UUID, which can find the specific request content that triggers the vulnerability according to
  the dnslog record

### Log4j automatic active scanning

- Get all requests for automatic page acquisition through chrome headless + crawler, and import the requests into the
  passive proxy to realize automatic scanning

### Log4j Scanning Readme

- [English](https://www.yuque.com/vipersec/blog/sn2x39)

## v1.5.9 20211204

### Optimization

- Merge Metasploit Framework version 6.1.18
- Update ruby version to 3.0

### Bugfix

- Fix bug on FOFA search

## v1.5.8 20211126

### New features

- New module `Syscall Visual Studio project`

### Optimization

- `InternetScan` UI is updated to make the operation more convenient, and the manual import function is added
- Add partial log (heartbeat data section)
- Merge Metasploit Framework version 6.1.17

### Bugfix

- Fix the problem that the PEM certificate could not be loaded

## v1.5.7 20211115

### Optimization

- 'InternetScan' add debug interface
- Webdelivery currently no longer forces binding of target and payload
- Functional optimization of Puma and ipgeo
- front-end interaction optimization
- Merge Metasploit Framework version 6.1.15

### Bugfix

- Fix the handler exception caused by ipgeo exception
- Fix the repeated addition of UDP handler after Viper restart

## v1.5.6 20211031

### New Features

- Added 'Hander firewall' function
- Added the module of "Direct windows syscall evasion technique"

### Optimization

- reverse_http(s) when the network is disconnected, the timeout is updated from 21 seconds (Windows default) to 3
  seconds
- The current session does not expire by default and will not exit automatically
- Merge Metasploit Framework version 6.1.13

### Bugfix

- Repair reverse_tcp failed to connect when 'sessionexpirationtimeout' is 0
- Fix failure to get default lhost parameter on ui

## v1.5.5 20211024

### New Features

- Added `CVE-2021-40449 LPE` module
- One click download all Viper logs from WEBUI

### Optimization

- Merged metasploit-framework 6.1.12

### Bugfix

- Fix the port occupancy problem after the socks is removed

## v1.5.4 20211017

### New Features

- Added `MS17-010 Exploit (CSharp)` module

### Optimization

- Merged metasploit-framework 6.1.11

### Bugfix

- Fix duplicate add reverse_http(s) handler failed to deal with session online requests.

## v1.5.3 20211010

### Optimization

- Optimize msfconsole user experience
- Merged metasploit-framework 6.1.10

<br/>

## v1.5.2 20211007

### Optimization

- Login page multilingual support
- Merged metasploit-framework 6.1.9

## v1.5.1 20210926

### New Features

- Added `Obtain Internet outbound IP` module
- New search filter for session process list

### Optimization

- Antivirus software display supports English version
- Optimize the output format of the intranet scanning module
- Optimize the performance and UI of the `Run Module` function
- Merged metasploit-framework 6.1.8 version

### Bugfix

- Fix the problem that the name of antivirus software is not displayed

## v1.5.0 20210919

### New Features

- VIPER now support English language

### Optimization

- Optimized the format of session online SMS
- Merged metasploit-framework 6.1.7 version

### Bugfix

- Fixed the issue that `ExitOnSession` did not take effect
- Fix the issue that the bind handler of the exploit module does not take effect

## v1.4.2 20210822

### New Features

- Added `Session online by SCF (Tencent API Gateway)` module

### Optimization

- Use Unix socketpair to replace 127.0.0.1 socketpair to improve performance
- Optimize the `handler` function, add HttpHostHeader parameter
- Block ids check of session
- Merged metasploit-framework 6.1.5 version

### Bugfix

- Fixed the problem that some module tasks could not be deleted
- Fixed the issue of channel not being released in MSF
- Fix the issue of `Clone Https certificate` certificate length, adapt to the new features of SSLVersion
- Fix the issue that the session does not respond after the use of Linux intranet routing and command execution due to
  stream hang

</details>

# FAQ

- [FAQ](https://www.yuque.com/viper-en/faq)

# Issues

- github issues : [https://github.com/FunnyWolf/Viper/issues](https://github.com/FunnyWolf/Viper/issues)

# Modules

- [Document link](https://www.yuque.com/viper-en/module)

# System architecture diagram

![viper.png](https://cdn.nlark.com/yuque/0/2021/png/159259/1627364231093-768d3b07-e044-4a2d-a3fa-e9ebd92a0828.png)

# Development

- [Development](https://www.yuque.com/viper-en/code)

# Thanks

Edward_Snowdeng exp
[Fnzer0](https://github.com/Fnzer0)
[qingyun00](https://github.com/qingyun00)
脸谱 NoobFTW Somd5-小宇
[timwhitez](https://github.com/timwhitez)
[ViCrack](https://github.com/ViCrack)
[xiaobei97](https://github.com/xiaobei97)
[yumusb](https://github.com/yumusb)

# 404StarLink 2.0 - Galaxy

![](https://github.com/knownsec/404StarLink-Project/raw/master/logo.png)

Viper has joined 404Team [404StarLink 2.0 - Galaxy](https://github.com/knownsec/404StarLink2.0-Galaxy)

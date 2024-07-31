---
title: "进程、线程和协程"
description: ""
date: 2024-07-29T22:19:50+08:00
lastmod: 2024-07-29T22:19:50+08:00
draft: true
showToc: true
weight: false
categories: ["android", "system", "rust"]
tags: ["android", "process", "thread", "coroutine", "kotlin", "rust", "tokio"]
---

## TLDR

|     | 进程 | 线程 | 协程 |
| --- | --- | --- | --- |
| 基本概念 | 系统资源分配的最小单位 (承载应用) | 系统调度的最小单位 | 线程上的任务单元 |
| 控制者 | 系统 | 系统 | 语言/框架/应用程序 |

## 进程 Process

### 进程内存结构

#### Out Of Memory (OOM)

### 僵尸进程/孤儿进程

### 进程间通信 Inter-process Communication (IPC)

### Android 中的 IPC

#### Intents

#### Messenger

#### Shared Preference

#### Content Provider

#### Broadcast Receiver

#### Binder (AIDL)

## 线程 Thread

### CPU 时间片

### Java 线程优先级

### 线程间竞争 Racing Condition

### Rust 线程同步

#### 互斥锁 Mutex

#### 读写锁 RwLock

#### 条件变量 Condition Variable (CondVar)

#### 信号量 Semaphore

### Kotlin 线程同步

#### Syncronized

#### Volatile 关键字

#### Mutex

#### ReentrantLock

#### BlockingQueue

#### CountDownLatch

#### CAS

### Android 线程 Looper, MessageQueue 和 Handler

#### 同步屏障 SyncBarrier

## 协程 Coroutine

### Kotlin 协程

#### 调度器 Dispather

#### 挂起与恢复

#### Kotlin 协程异常处理

### Rust Tokio 异步框架

#### Future trait 和 await
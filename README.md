# AI Coding Agents Guide

Claude Code, Pi, OpenCode 가이드 (부서 폐쇄망 인프라 한정 설명, 2026년 7월 13일에 작성)
엄밀한 설명보다는 우리 파트에서 사용 가능한 AI Agent를 다루기 위한 최소 설명으로 구성되어 있습니다.

---

## 목차

- [1. AI Agent](#1-ai-agent)
  - [1.1. AI Agent](#11-ai-agent)
  - [1.2. Model](#12-model)
  - [1.3. Context Window](#13-context-window)
- [2. Claude Code](#2-claude-code)
  - [2.1. Claude Code](#21-claude-code)

## 1. AI Agent

### 1.1. AI Agent
챗봇은 채팅창 안에 머무르지만 코드 에이전트는 터미널과 파일 시스템을 통해 개발 작업을 수행합니다.
Read, Write, Edit, Bash 등 다양한 도구를 사용합니다.

### 1.2. Model
AI Agent를 얘기할 때 Model이란 Large Language Model(LLM)을 의미합니다.
LLM은 다시 Text-Only와 Multimodal LLM으로 나뉩니다.

챗봇과 대화할 때 다양한 모델을 선택할 수 있습니다.
마찬가지로 같은 에이전트라도 다른 모델로 구동할 수 있습니다.

일반적으로 에이전트를 몸에 비유하고 모델을 뇌에 비유합니다.
또 다른 비유로, 에이전트가 비행기나 선박이라면 모델은 그것들을 구동하는 엔진이라고 볼 수 있겠죠.

### 1.3. Context Window
Model이 수용할 수 있는 내용(Context Window)은 한계가 있습니다. 이 수용 한계는 토큰(token)의 숫자로 정의됩니다. 2026년 7월 기준 모델에 따라 다르며, 대표적인 수치로 128K, 256K, 1M 토큰 등이 있습니다.

> *"Context Window가 한계에 도달하면 잘라내기(Truncation), 요약(Summarization), 제거(Eviction) 등의 방법으로 대응해야 합니다."*

## 2. Claude Code

### 2.1. Claude Code
우리 파트에서는 `claude-adtco`를 입력해서 실행 가능합니다. 2026년 7월 13일 기준 `r71` 버전 이하라면, `claude-adtco --restart`로 패치하거나, 실행중인 모든 Claude Code를 종료한 뒤, `claude-adtco` 입력 시 최신 버전으로 업데이트됩니다.

세 에이전트 중 가장 복잡하고 정교합니다. 수많은 도구와 부가기능을 통해 모델의 작업을 돕습니다. 단, Anthropic 모델에 최적화되어 있으므로 서드파티 모델 사용 시 도구 사용 성공률이 낮아지며 일부 도구가 호환되지 않습니다.

### 2.2. 슬래시 명령어






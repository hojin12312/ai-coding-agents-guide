# AI Coding Agents Guide

Claude Code, Pi, OpenCode 가이드 (부서 폐쇄망 인프라 한정 설명, 2026년 7월 13일에 작성)
엄밀한 설명보다는 우리 파트에서 사용 가능한 AI Agent를 다루기 위한 최소 설명으로 구성되어 있습니다.

---

## 목차

## 1. AI Agent

### 1.1. AI Agent
챗봇은 채팅창 안에 머무르지만 에이전트는 터미널로 PC를 제어합니다.
Read, Write, Edit, Bash 등 다양한 도구를 사용합니다.

### 1.2. Model
AI Agent를 얘기할 때 Model이란 Large Language Model(LLM)을 의미합니다.
LLM은 다시 Text-Only와 Multimodal LLM으로 나뉩니다.

챗봇과 대화할 때 다양한 모델을 선택할 수 있습니다.
마찬가지로 같은 에이전트라도 다른 모델로 구동할 수 있습니다.

일반적으로 에이전트를 몸에 비유하고 모델을 뇌에 비유합니다.
에이전트가 비행기, 선박, 기차, 자동차라면 모델은 그것들을 구동하는 엔진이라고 볼 수도 있겠죠.

### 1.3. Context Window
Model이 수용할 수 있는 내용(Context Window)은 한계가 있습니다. 이 한계는 토큰(token)의 숫자로 정의됩니다.
2026년 7월 기준 중형 모델은 일반적으로 256K 토큰까지, 그보다 큰 모델은 1M 토큰까지 수용할 수 있습니다.

무한히 작업을 이어가기 위해서는 한계에 도달하기 전 Context를 압축해야 합니다.

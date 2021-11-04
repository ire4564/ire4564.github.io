---
title: "[FE] Browser Rendering"
layout: post
date: 2021-11-04 19:05
image: /assets/images/markdown.jpg
headerImage: false
tag:
- markdown
- elements
star: false
category: blog
author: ire4564
description: Markdown summary with different optionsBasic formatting브
---





## Brower Rendering의 원리

브라우저가 화면에 나타내는 요소를 렌더링할 때, 렌더링 엔진을 사용한다. 이 때, CRP(Critical Rendering Path)라는 프로세스를 채용하며 다음 단계들로 이루어진다.



1. HTML 파싱 후, DOM 트리를 구축한다.
2. CSS 파싱 후, CSSOM 트리를 구축한다.
3. JavaScript를 실행한다. (주의: HTML 중간에 스크립트가 있을 경우 HTML 파싱이 중단된다.)
4. DOM과 CSSOM을 조합하여 렌더 트리(Render Tree)를 구축한다.
5. 뷰 포트 기반으로 렌더트리의 각 노드가 가지는 정확한 위치와 크기를 계산한다. (Layout/Reflow)단계
6. 계산한 위치 및 크기를 기반으로 화면에 그리는 Paint 단계를 거친다.
7. 

-----


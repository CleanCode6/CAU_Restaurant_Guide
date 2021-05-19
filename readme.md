# Project Overview
"중앙대학교 맛집 추천 가이드"(CAU Restaurant Guide) 프로젝트 설계와 관련한 문서를 정리한 Repository 입니다. 

본 프로젝트는 [IntelligentTouristGuide](https://nevonprojects.com/intelligent-tourist-guide) 프로젝트를 참고하였습니다.

## Problem & Scenario
 중앙대학교에 많은 식당들이 있습니다, 그러나 사용자 개인에 맞게 식당들을 추천해주는 마땅한 앱이 없습니다. 따라서 학교 근처의 식당 정보들을 음식의 종류와 평가에 따라서 추천을 받을 수 있고, 사용자의 현재 위치기준에 근거해서 맛집 정보를 알려줄 수 있는 식당이 필요합니다. 따라서 각자 개인의 취향에 맞는 학교(또는 내 위치) 에서 가까운 맛있는 음식점을 추천하는 어플리케이션이 필요로합니다.

 해당 어플리케이션의 사용자는 **이용자** 와 **관리자** 2가지로 나뉩니다. 이용자는 어플리케이션에 회원가입 후 로그인 하여 음식점 추천 리스트 및 음식점 정보를 확인합니다. 관리자는 서비스에 접속 후 기본으로 설정된 관리자 계정으로 로그인하여 메인화면에 접속하고 음식점 추가 및 수정할 수 있습니다.

## Requirements
 요구사항은 Agile Process의 User Stroy 형식으로 명세되어 있습니다. 각 요구사항은 REQ-N(REQ-01, REQ-02, ...) 형식으로 명명했습니다.

## Usecase
 요구사항으로 부터 총 10가지의 유스케이스를 명세하였으며, 각 유스케이스는 UC-N(UC-01, UC-02, ...) 형식으로 명명했습니다.

 유스케이스 다이어그램에는 다음 Actor를 포함합니다.
 - 이용자
 - 관리자
 - DB 
 - 서버
 - 추천시스템
 - 지도

## Domain
 도메인 모델은 유스케이스로 부터 명세하였습니다. 

## Implementation & Detail
 설계의 구현을 위해 다음 3개의 서브 그룹으로 나누어 Standalone Demo가 가능하도록 구현하였습니다. 

 1. 회원가입/로그인
 2. 식당 추천/조회
 3. 식당 관리

 구현을 위해서 다음 기술 및 언어를 사용합니다.
 - 결과물의 형태: Web Application
 - 구현 언어: python
 - Framework: [flask](https://flask.palletsprojects.com/en/2.0.x/)

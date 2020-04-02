---
description: 증인노드 구축 가이드
---

# mira-p2p-0.22.5

## 작업 요약

* PC 준비하기

## 작업 사양

> P2P 노드 구축 기준으로 작업한 SPEC 입니다. FULL 노드 구성 시\( 추가되는 plugin 의 정보에 따라 다름 \)  최소 사양은 변경\(증가\)되니 참조 바랍니다

@dev.supporters 에서 사용한 GCP 정보는 아래와 같습니다.

* REGION : us-west1\(오리건\) / us-west1-b
* OS : Ubuntu 16.04
* E2 : e2-highmem-8\(vCPU8, 64GB RAM\)
* SSD 500GB

월 $348.97 예상 / 시간당 약 $0.478 \( v8 =&gt; v4 로 custom 셋팅 시 월 약 68$ 절감 가능 \)

## STEEM-TOOLKIT 설치

> @someguy123 이 제작한 steem-toolkit 을 활용하여 손쉽게 다양한 작업을 진행 할 수 있습니다.

### 특징

* docker 자동 설치
* 손쉽게 docker image 적용 가능
* 공유메모리\(/dev/shm\) 설정 가능
* 2001 포트\(seed\) 자동 포워딩
* 시드노드\(seed node\) 풀노드\(full node\) 관련 기본 설정 정보 제공
* 빠르게 start, stop, replay rebuild, local wallet 등의 작업 수행

### 설치

> 설치 이후 `steem-docker` 폴더에서 작업을 진행 합니다.

```text
git clone https://github.com/someguy123/steem-docker.git
```

### 도커 설치

> 이미 도커가 설치 된 경우에는 해당 작업을 건너 뛰어도 상관 없습니다.

```text
./run.sh install_docker
```

### 도커 이미지 다운로드

> [https://hub.docker.com/r/someguy123/steem/tags](https://hub.docker.com/r/someguy123/steem/tags) 링크를 참조하여 도커 이미지를 다운로드 받습니다.

{% embed url="https://hub.docker.com/r/someguy123/steem/tags" %}

```text
docker pull someguy123/steem:v0.22.5
```



## 참조링크

* [https://que.com/howto-setup-a-steem-witness-node/comment-page-1/](https://que.com/howto-setup-a-steem-witness-node/comment-page-1/)
* [https://github.com/Someguy123/steem-docker](https://github.com/Someguy123/steem-docker)
* [https://hub.docker.com/r/someguy123/steem/tags](https://hub.docker.com/r/someguy123/steem/tags)




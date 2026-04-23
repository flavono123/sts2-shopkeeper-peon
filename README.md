# sts2-shopkeeper-peon

Slay the Spire 2 **상점 주인**(Merchant)과 **짭상인**(Reverse Merchant) 보이스로 만든 [OpenPeon / peon-ping](https://openpeon.com) 사운드 팩.

어허, 아하, 으 — Claude Code 세션 내내 상점 주인이 반응한다.

## Install

로컬에서 테스트:
```sh
peon packs install-local /path/to/sts2-shopkeeper-peon
peon packs use sts2_shopkeeper
peon preview session.start
```

## 카테고리 매핑

| CESP 카테고리      | 의도              |
|-------------------|-------------------|
| `session.start`   | 인사 / 손님맞이     |
| `task.acknowledge`| 주문 받음 / 네네   |
| `task.complete`   | 거래 완료          |
| `task.error`      | 어허 (꾸중/불만)    |
| `input.required`  | 으 (뜸들임/고민)    |
| `resource.limit`  | 재고/골드 부족     |
| `user.spam`       | 짭상인 (reverse merchant) |

## License

- 팩 manifest/스크립트: **CC-BY-NC-4.0**
- 오디오 에셋: Slay the Spire 2 © Mega Crit. 팬메이드 비상업적 재배포 가정.
  게임사 요청 시 내립니다.

## Source

오디오는 STS2 게임 PCK(`Slay the Spire 2.pck`)에서 [GDRE Tools](https://github.com/GDRETools/gdsdecomp)로 추출한 `merchant/*.wav`, `reverse_merchant/*.wav` 리소스.

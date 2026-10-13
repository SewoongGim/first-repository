# B550M 메인보드 조사 (Wi-Fi 없는 모델)

- 조사 시각: 2026-10-13 (KST 오후 7시경)
- 목적: AM4 게이밍 PC (Ryzen 5 5600 → Ryzen 7 5700X3D 예정), 미니타워 M-ATX, 360mm AIO(펌프+팬3) + 케이스 팬3
- 필수 조건: 전면 USB Type-C 헤더, BIOS Flashback, 펌프 헤더, USB 2.0 헤더(LCD 펌프용), ARGB 5V 헤더 수, B550 (A520 제외)

## 1. 사양 비교 (공식 확인 범위)

범례: "확인" = 공식 스펙 페이지 또는 리테일러 요약에서 확인, "미확인" = 조사 수단 차단 또는 자료 없음.

| 항목 | MSI MAG B550M MORTAR (Wi-Fi 없음) | ASUS TUF GAMING B550M-PLUS (Wi-Fi 없음) | ASRock B550M Pro4 |
|---|---|---|---|
| 출처 | 공식 페이지 403 차단. 리테일러 요약 (adorama, buildcores, tlggaming 등) | 공식 스펙 https://www.asus.com/motherboards-components/motherboards/tuf-gaming/tuf-gaming-b550m-plus/techspec/ (확인) | 공식 페이지 Incapsula 차단. 검색 요약 (paradigit, pccasegear, tecisoft 등) + 매뉴얼 https://download.asrock.com/Manual/B550%20Pro4.pdf (미열람) |
| 전면 USB Type-C 헤더 | **있음** (내부 USB 3.2 Gen1 Type-C 1개, 리테일러 요약) | **없음** (내부 USB 3.2 Gen1 헤더 1개 = 포트 2개, 확인) | **확인 못 함** (검색 요약상 후면 USB 3.2 Gen2 Type-C 1개만 언급) |
| BIOS Flashback | **있음** 버튼 (후면 I/O, 리테일러 요약) | **있음** "BIOS FlashBack 버튼" (후면, 확인) | **미확인** (Pro4 공식 자료 차단) |
| 펌프 헤더 | PUMP_FAN 4-pin 1개 (리테일러 요약) | 공식 스펙에 펌프 명칭 없음. CPU_OPT 헤더 (매뉴얼 미열람) | "CPU/Water Pump" 1개 (검색 요약) |
| 팬 헤더 총수 | **미확인** (요약에 개수 없음) | **4개** = CPU_FAN 1 + CPU_OPT 1 + CHA_FAN 2 (확인) | **6개** = CPU_FAN 1 + CPU/Water Pump 1 + Chassis/Water Pump 4 (검색 요약) |
| ARGB 5V 3-pin | **미확인** | **1개** (Addressable Gen2) (확인) | **2개** (5V 3A 등급, 검색 요약) |
| RGB 12V 4-pin | **미확인** | **2개** (Aura RGB Strip) (확인) | **2개** (12V 3A 등급, 검색 요약) |
| USB 2.0 내부 헤더 | **미확인** | **2개** (추가 USB 2.0 4포트) (확인) | **2개** (4포트) (검색 요약) |
| USB 3.2 Gen1 내부 | Type-C 1 + 헤더 1 (+2포트) (요약) | 헤더 1 (+2포트) (확인) | 헤더 2 (4포트) 다만 요약 1건은 1개 (불일치) |
| M.2 슬롯 | **미확인** (요약상 2개 언급) | **2개**: M.2_1 PCIe 4.0 x4 / M.2_2 PCIe 3.0 x4 (확인) | **미확인** |
| SATA | **미확인** | **4개** (확인) | **미확인** |
| PCIe x16 | **미확인** | PCIe 4.0 x16 (x16 모드) 1 + PCIe 3.0 x16 (x4 모드) 1 (확인) | **미확인** |
| 5600 지원 최소 BIOS | 미확인 (MSI 공식 차단) | **2423 GO** (ASUS CPU 목록 "Validated since BIOS", https://www.asus.com/motherboards-components/motherboards/tuf-gaming/tuf-gaming-b550m-plus/helpdesk_cpu/) | 미확인 |
| 5700X3D 지원 최소 BIOS | 미확인 | **2803 GO** (동일 출처) | 미확인 |
| VRM 방열판 높이 | 자료 없음 | 자료 없음 | 자료 없음 |

참고:
- ASUS CPU 목록의 "Validated since BIOS"는 검증된 최소 BIOS이며 실제 구버전 출고 시 BIOS 업데이트 필요.
- 5700X3D (2024-01 출시)는 2024년 이전 출고 재고에 구버전 BIOS가 들어있을 가능성이 높음. 구매 시 BIOS 버전 확인 필요. 구버전이면 Flashback으로 CPU 없이 갱신 가능 (ASUS, MSI 모두 Flashback 있음).
- MSI MORTAR 공식 페이지와 ASRock Pro4 공식 페이지가 차단되어 세부 항목 일부는 리테일러 요약 기준. 매뉴얼 확인 필요.

## 2. 가격 (2026-10-13 조회)

### 2-1. 신품

| 플랫폼 | 상품 | 신품/중고 | 가격 | 배송비 | 실구매가 | 조건 | 링크 | 비고 |
|---|---|---|---|---|---|---|---|---|
| Danawa (오퍼) | ASUS TUF GAMING B550M-PLUS STCOM (pcode 11571368) | 신품 | 149,000 | 0 (컴나무) | 149,000 | **조건부가: 현금 결제** (is_conditional_price=True, label=현금) | https://prod.danawa.com/info/?pcode=11571368 | 다른 판매처 151,500~154,000 (배송비 포함). 단종 여부 표시 없음 |
| Danawa (오퍼) | 동 상품, 판매처 하나컴 | 신품 | 151,000 | 3,000 | 154,000 | 현금 조건부 | 동일 | |
| Coupang (파트너스) | ASUS TUF Gaming B550M-PLUS STCOM | 신품 | 243,300 | - | 243,300 | 일반 | https://a.retn.kr/s/C43Nv3l | 고가 |
| Coupang | 에이수스 TUF GAMING B550M-PLUS | 신품 | 161,500 | - | 161,500 | 일반 | https://a.retn.kr/s/YUJ166S | |
| Coupang | ASRock B550M Pro4 (국내 정규 대리점품) | 신품 | **102,140** | - | 102,140 | 일반 | https://a.retn.kr/s/yc8yJe2 | 최저 신품 |
| Coupang | ASRock B550M Pro4 (별도 판매처) | 신품 | 157,600 | - | 157,600 | 일반 | https://a.retn.kr/s/RhUodoj | |
| Enuri | ASRock B550M Pro4 | 신품 | 102,140 | - | 102,140 | 일반 (Coupang 연동 광고 링크) | https://www.enuri.com/search.jsp?keyword=B550M+Pro4 | |
| Danawa (오퍼) | ASRock 제품군 (Pro RS, Pro-A 등 Pro4 아님) | 신품 | 107,790~123,850 | - | - | 참고 | 검색 결과만 | Pro4 카탈로그는 Danawa 검색에서 찾지 못함 |
| Coupang | MSI MAG B550M MORTAR MAX WIFI | 신품 (Wi-Fi) | 187,200 | - | 187,200 | 참고용 Wi-Fi | https://a.retn.kr/s/QktIuWw | Wi-Fi 모델 |
| Danawa (오퍼) | MSI MAG B550M MORTAR WIFI6E 등 (TH201/EE128/EE715) | 신품 (Wi-Fi) | 175,610~197,320 | - | - | 참고용 Wi-Fi | https://prod.danawa.com/info/?pcode=11578325 (박격포 WiFi 카탈로그) | Wi-Fi 버전 |
| Danawa | MSI AM4 mATX MAG B550M MORTAR (제목에 WIFI 없음) | 신품 | 220,100 | - | - | **비Wi-Fi 여부 불명확**, 판매처 목록 조회 실패 | https://prod.danawa.com/bridge/go_link_goods.php?cate_c1=861&cate_c2=880&cate_c3=997&cate_c4=0&cmpny_c=TH201&link_prod_c=9673832309 | 확인 필요 |
| Danawa | MSI MAG B550M 박격포 (비Wi-Fi 카탈로그) | - | - | - | - | 카탈로그 검색 결과 없음 | - | 비Wi-Fi 신품 확인 실패 |
| Danawa (오퍼) | GIGABYTE B550M AORUS ELITE (참고, 후보 아님) | 신품 | 114,860 (피씨디렉트) / 115,980 (제이씨현) | - | - | 참고 | https://prod.danawa.com/info/?pcode=11684576 | 대안 참고용 |

### 2-2. 중고

| 플랫폼 | 상품 | 신품/중고 | 가격 | 배송비 | 실구매가 | 조건 | 링크 | 비고 |
|---|---|---|---|---|---|---|---|---|
| Danawa (중고 리스트) | [중고] MSI MAG B550M 박격포 (무상 1달, 라이젠 4세대 지원) | 중고 | 109,130 | 미확인 | 미확인 | 판매자 EE128 | https://prod.danawa.com/bridge/go_link_goods.php?cate_c1=58751&cate_c2=58760&cate_c3=0&cate_c4=0&cmpny_c=EE128&link_prod_c=4382004083 | 무상 1달, 박스 미확인 |
| Danawa (중고 리스트) | [중고] MSI MAG B550M 박격포 (동일 조건) | 중고 | 112,500 | 미확인 | 미확인 | 판매자 EE715 | https://prod.danawa.com/bridge/go_link_goods.php?cate_c1=861&cate_c2=875&cate_c3=0&cate_c4=0&cmpny_c=EE715&link_prod_c=F562518319 | 동일 |
| Bunjang | MSI MAG B550M MORTAR DDR4 메인보드 (비Wi-Fi 표기) | 중고 (사용감 없음) | 129,000 | 일반 5,000 | 134,000 | 택배 가능, 수원 장안구, 최신 BIOS 업데이트 완료 명시, 1시간 전 등록 | https://m.bunjang.co.kr/products/439432194 | 최저 중고 가격 대비 높음 |
| Bunjang | ASRock B550M Pro4 | 중고 (사용감 적음) | 95,000 | 일반 3,000 | 98,000 | 홈서버 사용, BIOS 업데이트 완료, I/O 실드·쿨러 백플레이트 포함, **반품 불가** 명시 | https://m.bunjang.co.kr/products/438247883 | 최저 중고 |
| Bunjang | 애즈락 B550M PRO4 | 중고 (사용감 적음) | 95,000 | 일반 4,000 | 99,000 | 바이오스 최신 업데이트, 안전결제 | https://m.bunjang.co.kr/products/436894791 | |
| Bunjang | ASRock B550M PRO4 메인보드 | 중고 (사용감 적음) | 110,000 | 무료 | 110,000 | 택배·직거래 (청파동), 잘 작동 | https://m.bunjang.co.kr/products/438289648 | |
| Bunjang | MSI B550M 메인보드 판매 (모델 상세 불명, 5600X 사용) | 중고 | 80,000 | 일반 4,000 | 84,000 | **모델 불명확** (MSI B550M 중 어떤 모델인지 미상) | https://m.bunjang.co.kr/products/439771750 | 확인 필요 |
| Bunjang | 라이젠5 5600X MSI MAG B550M MORTAR WIFI | 중고 (Wi-Fi) | 273,000 | - | - | 참고 Wi-Fi | https://m.bunjang.co.kr/products/436518061 | 제외 |
| Bunjang | 라이젠 5900x b550m 박격포 와이파이 | 중고 (Wi-Fi) | 450,000 | - | - | 참고 Wi-Fi, 고가 | https://m.bunjang.co.kr/products/438952002 | 제외 |
| Daangn | - | - | - | - | - | **실패**: 스크립트 응답이 JSON 아님 (daangn.com API 차단 추정) | - | |
| 중고나라/퀘이사존/쿨엔조이 | - | - | - | - | - | 미시도 (시간 제약) | - | |

## 3. 조회 실패/제약
- Naver Shopping: 조정자 지시에 따라 생략 (Aside 등 브라우저 사용 금지 지시).
- 공식 스펙 페이지: MSI MORTAR (403), ASRock Pro4 (Incapsula 차단). ASUS는 curl `--ssl-no-revoke` 옵션으로 조회 가능 (Schannel 폐기 확인 오류 우회).
- Daangn: 스크립트가 JSON이 아닌 응답을 받아 실패 (불당동/효자동 모두 동일).
- Danawa 카탈로그: ASRock B550M Pro4 카탈로그 미발견, MSI MORTAR 비Wi-Fi 신품 미발견.
- 번개장터 `item get` 결과는 JSON 내 price 필드 오염 (가격은 title/item.price 사용).
- 에누리: 가격 파싱 일부만 성공 (노이즈 많음).

## 4. 권장 (요약)
- 필수 조건 충족 측면에서 MSI MAG B550M MORTAR (전면 USB Type-C, Flashback, 펌프 헤더 확인) 유력. 단 팬 헤더 총수·ARGB 개수 미확인 → 구매 전 MSI 매뉴얼 확인 필요.
- ASUS TUF B550M-PLUS: 스펙 확인 완료. 전면 USB-C 없음, 팬 헤더 4개 (펌프+팬3 동시 연결 시 부족할 수 있음). 신품 최저 149,000 (현금 조건부).
- ASRock B550M Pro4: 팬 헤더 6개로 펌프+팬 다수에 유리하나 전면 USB-C 헤더 미확인, Flashback 미확인. 최저 신품 102,140, 최저 중고 95,000.
- 공통: 5700X3D 대응을 위해 BIOS 2803 GO 이상 (ASUS 기준) 확인 필요. 구매 시 판매자에게 BIOS 버전 문의.

# AirJoule (AIRJ) - Supply Chain Expert 분석
## 에이전트 08: 공급망/소재 전문가

**판정: 우려 🔴**

## PERSONA 8:공급망/소재 전문가 분석

### "AirJoule의 밸류체인 해부: MOF에서 현장 배치까지"

**작성자: 원자재-최종제품 밸류체인 분석 전문가**

---

### 1. MOF 원재료 공급: BASF의 대량 생산 능력과 비용

**BASF의 MOF 생산 현황:**

BASF는 2023년 **세계 최초로 MOF의 상업적 규모 생산**을 달성한 기업이다. 주요 사항:

- **생산 규모**: CALF-20(탄소 포집용 MOF)를 **연간 수백 톤(several hundred tonnes/year)** 규모로 생산 가능
- **글로벌 생산 인프라**: 전 세계 여러 사이트에서 맞춤형 MOF 생산 가능
- **비용 절감 전략**: 실험실 레시피를 그대로 확대하는 것이 아니라, "스케일업 과정에서의 단순화(simplification during scale-up)"와 "적절한 설비에서의 제조(manufacturing in the right assets)"를 통해 비용 효율성 확보
- BASF의 기존 촉매/흡착제 사업 인프라를 활용하여 MOF 전용 신규 투자 최소화

**MOF 제조 비용 분석:**

| 생산 규모 | 예상 비용 ($/kg) | 비고 |
|-----------|-----------------|------|
| 연간 100톤 | ~$55/kg | 현재 중규모 생산 수준 |
| 연간 1,000톤 | ~$29.5/kg | 본격 양산 시 |
| 장기 목표 | $10/kg 미만 | 공정 최적화 후 |
| 현재 소량 생산 | $250~1,800/kg | 연구용/소규모 |
| 상용 벤치마크(제올라이트 13X) | $1.5~3/kg | MOF의 경쟁 소재 |

**핵심 과제**: 현재 MOF 비용은 전통적 흡착제(제올라이트) 대비 **10~20배** 비싸다. BASF-AirJoule 공동 개발을 통해 "상업적으로 실행 가능한 비용(commercially viable cost)"까지 절감했다고 발표했으나, 구체적인 단가는 비공개다. 양산 시 $10~30/kg 수준이 목표로 추정되며, 이 범위에 도달하면 데이터센터 WPA(Water Purchase Agreement) 모델의 경제성이 확보될 수 있다.

---

### 2. AirJoule 시스템 제조 공급망: 핵심 부품 분석

**시스템 아키텍처:**

AirJoule 시스템은 크게 5개 핵심 모듈로 구성된다:

1. **MOF 흡착재**: BASF 공급, GE Vernova의 독점 코팅 공정 적용
2. **이중 진공 챔버(Dual Vacuum Chamber)**: 흡착/탈착을 동시에 수행하는 핵심 하드웨어
3. **진공 펌프 시스템**: 챔버 내 압력을 낮춰 MOF에서 수증기 탈착 유도
4. **열교환기**: 데이터센터 폐열을 시스템으로 전달
5. **제어/자동화 시스템**: 24/7 무인 운영을 위한 센서 및 소프트웨어

**제조 거점:**
- **Newark, Delaware**: 42,000 sq ft(약 3,900m2) 제조시설, 2024년 말 가동 시작
- 35,000 sq ft의 흡착재 코팅, 제조, 조립, 테스트 라인 구축
- 현재 약 **35명** 근무, 최대 **60명**까지 확대 계획 (화학 엔지니어, 화학자, 기술자 포함)

**제조 단계별 공급망:**

```
[BASF] → MOF 원재료 → [GE Vernova JV] → 흡착재 코팅 →
[AirJoule JV] → 시스템 조립/테스트 →
[현장 설치] → 데이터센터/산업시설
```

---

### 3. 스케일업 시 병목 포인트 분석

대량 생산을 제한할 수 있는 핵심 병목을 우선순위별로 분석한다.

**병목 #1: MOF 소재 자체 (심각도: 높음)**
- 전 세계적으로 연간 100톤 이상 MOF 생산이 가능한 시설은 **20~30개**에 불과
- 90,000종 이상 알려진 MOF 구조 중 산업적 양에서 활용 가능한 것은 **120종 미만**
- 고순도 링커(linker) 공급망 제약이 MOF 제조업체의 **18~25%**에 영향
- 전통적 용매열 합성법은 100~250도C, 고순도 용매, 12~48시간 반응 시간이 필요하여 양산 시 운영 비용 상승
- 펠릿화(pelletization) 과정에서 다공성이 **10~25% 감소**, 용매 회수 공정 추가 시 시설 비용 **18~26% 증가**

**병목 #2: 이중 진공 챔버 제조 (심각도: 중-높음)**
- 고정밀 진공 챔버는 **스테인리스 스틸, 알루미늄, 특수 밀봉재**를 사용하며, 정밀 용접, 가공, 누설 시험이 필요
- 맞춤형 설계가 불가피하여 표준화 및 대량 생산이 어려움
- 2025년 미국의 새로운 관세 정책으로 수입 강재, 센서, 전자 모듈의 비용 압력 증가
- 현재 Delaware 시설은 프리프로덕션 수준이며, 연간 수백~수천 대 생산을 위한 설비 확장이 필요

**병목 #3: GE Vernova 흡착재 코팅 공정 (심각도: 중간)**
- GE Vernova의 독점 코팅 기술은 JV의 핵심 경쟁력이자 단일 공정 의존 리스크
- 코팅 공정의 수율(yield)과 처리량(throughput)이 전체 시스템 생산량을 결정
- 코팅의 균일성과 내구성이 시스템 성능에 직결

**병목 #4: 전문 인력 (심각도: 중간)**
- MOF 합성, 진공 기술, 흡착 공학 분야의 전문 인력 확보가 제한적
- 현재 35명에서 60명으로 확대해야 하나, 해당 분야 인력 풀이 작음

---

### 4. GE Vernova JV에서 GE의 역할 분석

GE Vernova는 이 JV에서 **핵심 소재 기술과 R&D 역량**을 담당한다.

**GE Vernova가 담당하는 부분:**

| 역할 | GE Vernova | AirJoule Technologies(Montana) |
|------|-----------|-------------------------------|
| **소재 기술** | 독점 흡착재(sorbent) 소재 제공 | - |
| **코팅 공정** | 독점 코팅 공정(coating process) | - |
| **시스템 설계** | - | 특허 보유 AirJoule 공정 및 시스템 |
| **R&D** | Advanced Research팀이 JV R&D 지원 | 시스템 엔지니어링 |
| **제조** | 공동 (Delaware 시설) | 공동 (Delaware 시설) |
| **투자** | 초기 $500만 투자 + 후속 지원 | $275만 자본 기여 (Q3 2025) |
| **지적재산** | 흡착재 관련 IP | 시스템/공정 관련 IP |

**지역별 사업권:**
- JV 독점 지역: **미주(Americas), 아프리카, 호주**
- 중동: TenX Investment 독점 유통 (JV 관할 밖으로 추정)

**GE Vernova의 전략적 가치**: GE의 글로벌 제조 인프라, 품질 관리 시스템, 공급망 관리 역량은 AirJoule의 스케일업에 결정적이다. 특히 GE Vernova가 에너지 인프라 분야에서 보유한 고객 네트워크는 데이터센터 및 발전소 시장 진입을 가속화할 수 있다. 다만 GE Vernova가 "유통"이나 "설치"를 직접 담당한다는 명시적 언급은 없으며, 현재까지는 **소재-코팅-R&D 중심의 기술 파트너** 역할에 집중하고 있다.

---

### 5. 경쟁사 대비 공급망 우위/열위

**우위 요소:**
- **BASF 파트너십**: 세계 최대 화학기업의 MOF 대량 생산 인프라에 접근 가능. 다른 AWG 스타트업은 자체 소재 생산에 의존하거나 소규모 공급업체에 의존
- **GE Vernova 브랜드**: 에너지 인프라 시장에서의 신뢰도, 품질 관리 시스템, 글로벌 서비스 네트워크
- **Carrier 파트너십**: HVAC 시장 진입 시 세계 최대 HVAC 제조사의 유통망 활용 가능. Carrier는 $1,000만 성장 자본 투자 약정
- **DOE(미국 에너지부) 협력**: 기술 상용화를 위한 정부 지원 확보
- **2025 노벨 화학상**: MOF 기초 연구에 수여되어 기술 인지도 및 신뢰도 상승

**열위 요소:**
- **제조 규모**: 42,000 sq ft 단일 시설은 프리프로덕션 수준. 경쟁사인 Aquaria는 $1.12억 자금 확보로 대규모 시스템 구축 중
- **공급망 길이**: MOF 원료 → BASF 합성 → GE 코팅 → JV 조립 → 현장 설치로 이어지는 다단계 체인은 리드타임 증가 요인
- **양산 검증 미완**: 프리프로덕션 시스템(일 1,000리터)에서 상업용 대규모 시스템으로의 전환이 아직 이루어지지 않음
- **수직 통합도 낮음**: 핵심 소재(BASF)와 핵심 공정(GE Vernova 코팅)을 외부에 의존

---

### 6. 단일 공급원(BASF) 의존 리스크

이 리스크는 **AirJoule 자체도 SEC 공시에서 명시적으로 인정**하고 있는 핵심 리스크다.

**리스크 분석:**

| 리스크 유형 | 세부 내용 | 심각도 |
|------------|---------|--------|
| 공급 중단 | BASF 생산시설 사고/정비 시 대체 공급원 부재 | 높음 |
| 가격 교섭력 | 단일 공급자 → 가격 인상 압력에 취약 | 중-높음 |
| 기술 종속 | BASF가 독자적으로 또는 경쟁사와 MOF 사업 확대 시 이해 충돌 | 중간 |
| 품질 변동 | MOF 배치(batch)간 품질 일관성이 시스템 성능에 직결 | 중간 |
| 지정학적 리스크 | BASF의 주요 생산거점이 유럽(독일 루트비히스하펜) → 유럽 에너지 비용/규제 리스크 | 낮음-중간 |

**완화 요소:**
- GE Vernova JV가 자체 흡착재 개발 역량을 보유 (GE Vernova의 독점 sorbent)하므로, BASF MOF와 GE 자체 sorbent 간의 이중화(redundancy)가 가능할 수 있음
- MOF 시장 자체가 성장 중(2034년까지 $6.85억 규모)이므로 BASF 외 공급자(Numat, Decarbontek 등) 등장 가능
- 그러나 현시점에서 AirJoule에 최적화된 특정 MOF를 생산할 수 있는 것은 **사실상 BASF가 유일**

**애널리스트 판단**: BASF 의존은 AirJoule의 **가장 심각한 공급망 리스크**다. 만약 BASF가 전략적으로 MOF를 AirJoule 경쟁사에게도 공급하기로 결정하거나, 자체 AWG 사업에 진출한다면, AirJoule의 경쟁 우위가 크게 훼손될 수 있다. 장기적으로 MOF 소재의 내재화(insourcing) 또는 복수 공급원 확보가 필수적이다.

---

### 7. 양산 시 목표 원가 vs 현재 원가 갭 분석

**현재 상황 (Pre-production, 2025):**
- A250 시스템: 일 250리터 생산 용량
- 프리프로덕션 시스템: 일 1,000리터 생산 목표 (2025년)
- 제조시설: 35,000 sq ft, 35명 인력
- 구체적 시스템 단가 미공개

**비용 구조 추정:**

AWG 업계 벤치마크에 따르면, 중형 상업용 AWG 한 대의 가격은 **$30,000~$50,000** 수준이다. AirJoule의 초기 시스템은 맞춤 제작 특성상 이보다 상당히 높을 것으로 추정된다.

| 비용 항목 | 현재 추정 | 양산 목표 | 비용 절감 경로 |
|----------|---------|----------|-------------|
| MOF 소재 | $30~55/kg | $10~15/kg | BASF 대량 구매 계약, 공정 최적화 |
| 진공 챔버 | 맞춤 제작 (고비용) | 표준화/대량 생산 | 설계 표준화, 금형 투자 |
| 진공 펌프 | 산업용 표준 부품 | 대량 구매 할인 | 비교적 소폭 절감 가능 |
| 열교환기 | 산업용 표준 부품 | 대량 구매 할인 | 비교적 소폭 절감 가능 |
| 조립/테스트 | 수동 조립 (높은 인건비) | 반자동화 라인 | 생산량 확대 시 단위당 비용 하락 |
| **총 시스템** | **추정 $100K+** | **목표 미공개** | 규모의 경제 + 학습 곡선 |

**Water Purchase Agreement(WPA) 경제성:**

AirJoule의 비즈니스 모델 중 WPA는 시스템 판매가 아닌 **물 판매**다. 이 경우:
- 데이터센터 운영자에게 리터당 또는 갤런당 장기 계약으로 물 공급
- CAPEX는 AirJoule이 부담하고, 운영 수익을 장기 회수
- 핵심 경제성 지표: 생산 물의 리터당 총비용(LCOW: Levelized Cost of Water) vs 대안(수도 요금, 담수화, 물 운송)

현재 미국 주요 도시의 산업용 수도 요금이 $2~8/1,000갤런인 반면, AWG의 물 생산 비용은 이보다 상당히 높다. AirJoule이 폐열을 무상으로 활용할 수 있다면 운영 비용을 대폭 절감할 수 있으나, **여전히 수도 요금 대비 프리미엄**이 존재할 것으로 보인다. 이 프리미엄을 정당화하려면: (1) 물 공급이 물리적으로 불가능한 지역, (2) 수자원 규제로 물 확보가 어려운 지역, (3) 물 부족으로 데이터센터 가동이 제한받는 상황에서 비즈니스 케이스가 성립한다.

---

### 8. 공급망 종합 리스크 매트릭스

| 리스크 요소 | 발생 확률 | 영향도 | 종합 등급 | 완화 전략 |
|-----------|---------|--------|---------|---------|
| BASF 공급 중단 | 낮음 | 매우 높음 | **높음** | 복수 MOF 공급원 개발, 안전 재고 확보 |
| MOF 비용 목표 미달 | 중간 | 높음 | **높음** | BASF와 장기 가격 계약, 대체 MOF 탐색 |
| 진공 챔버 확장 지연 | 중간 | 높음 | **중-높음** | 복수 제조업체 확보, 설계 표준화 |
| GE Vernova JV 갈등 | 낮음 | 높음 | **중간** | 명확한 JV 거버넌스, IP 보호 |
| 관세/무역 분쟁 | 중간 | 중간 | **중간** | 로컬 소싱 확대, 재고 선확보 |
| 전문 인력 확보 | 중-높음 | 중간 | **중간** | 대학 파트너십(ASU 등), 교육 프로그램 |
| 양산 품질 일관성 | 중간 | 높음 | **중-높음** | QC 시스템 고도화, GE 품질관리 프로세스 적용 |

---

### 9. 공급망 전문가 종합 투자 판단

**핵심 질문: AirJoule은 2026년 상업 배치 일정을 맞출 수 있는가?**

**긍정 요인:**
- BASF와 GE Vernova라는 세계적 수준의 파트너 확보는 스타트업으로서 이례적인 공급망 우위
- Delaware 제조시설이 가동 중이며, 프리프로덕션 시스템 생산 진행 중
- Nexus(텍사스), TenX(중동), ASU(애리조나), US Army ERDC(국방) 등 다양한 파일럿 채널 확보
- Q3 2025 기준 현금 $2,600만으로 "수년간의 운영 자금(multiple years of runway)" 보유

**우려 요인:**
- 프리프로덕션에서 양산까지의 "죽음의 계곡(Valley of Death)"을 아직 넘지 못함
- 42,000 sq ft 단일 시설로 대규모 데이터센터 수요를 충족하기에는 생산 능력이 절대적으로 부족
- 핵심 소재(MOF)와 핵심 공정(코팅)에 대한 외부 의존은 공급 리스크와 마진 압박 요인
- 2025년 매출 $0 상태에서 2026년 상업 매출 창출까지의 타임라인이 매우 촉박
- AWG 시스템의 리터당 비용이 기존 수자원 대비 경제적 우위를 확보했다는 검증이 부재

**결론**: AirJoule의 공급망은 **"세계적 파트너십으로 무장한 초기 단계 기업"**의 전형적 프로파일이다. 파트너의 역량은 최상급이나, 실제 양산-배치-수익화까지의 실행 리스크가 상당하다. 투자 관점에서는 2026년 하반기 Nexus 배치와 첫 WPA 매출이 가장 중요한 디리스킹(de-risking) 이벤트가 될 것이다.

---

**Sources:**
- [Data Centers and Water Consumption - EESI](https://www.eesi.org/articles/view/data-centers-and-water-consumption)
- [Data Center Water Usage: A Comprehensive Guide - Dgtl Infra](https://dgtlinfra.com/data-center-water-usage/)
- [WUE in Data Centers - Equinix Blog](https://blog.equinix.com/blog/2024/11/13/what-is-water-usage-effectiveness-wue-in-data-centers/)
- [PUE vs. WUE Balancing Efficiency - Attom Tech](https://attom.tech/pue-vs-wue-balancing-efficiency-and-sustainability-in-modern-data-centers/)
- [How AirJoule Plans to Extract Water from Data Center Waste Heat - DCD](https://www.datacenterdynamics.com/en/analysis/how-airjoule-plans-to-extract-water-from-data-center-waste-heat/)
- [AirJoule MOU with Nexus Data Centers - GlobeNewsWire](https://www.globenewswire.com/news-release/2025/12/02/3197885/0/en/AirJoule-Technologies-Identifies-Nexus-Data-Centers-as-AI-Hyperscale-Developer-and-Advances-Existing-MOU-Toward-First-Deployment-of-Onsite-Water-Purchase-Agreement-Using-Waste-Heat.html)
- [AirJoule $15M Investment by GE Vernova - GlobeNewsWire](https://www.globenewswire.com/news-release/2025/04/24/3067506/0/en/AirJoule-Technologies-Announces-15-Million-Investment-Anchored-by-GE-Vernova.html)
- [GE Vernova and Montana Technologies JV Close - PR Newswire](https://www.prnewswire.com/news-releases/ge-vernova-and-montana-technologies-close-joint-venture-to-manufacture-transformational-air-conditioning-and-atmospheric-water-harvesting-products-302084809.html)
- [BASF Industrial-Scale MOF Production - Chemical Processing](https://www.chemicalprocessing.com/industrynews/news/33012941/basf-delivers-industrial-scale-production-of-metal-organic-frameworks-for-carbon-capture)
- [BASF MOF Commercial Production - BASF](https://www.basf.com/global/en/media/news-releases/2023/10/p-23-327)
- [MOFs Industrialization Cost Assessment - RSC Faraday Discussions](https://pubs.rsc.org/en/content/articlelanding/2021/fd/d1fd00018g)
- [Metal-Organic Frameworks Market to $685M by 2034 - IDTechEx](https://www.idtechex.com/en/research-article/metal-organic-frameworks-market-to-grow-to-us-685-million-by-2034/30921)
- [AirJoule Delaware Manufacturing Facility - GlobeNewsWire](https://www.globenewswire.com/news-release/2025/08/04/3126548/0/en/AirJoule-Technologies-Cuts-the-Ribbon-at-Delaware-Manufacturing-Facility.html)
- [AirJoule Q3 2025 Results - Nasdaq](https://www.nasdaq.com/press-release/airjoule-technologies-nasdaq-airj-announces-third-quarter-2025-results-and-provides)
- [AirJoule FY2024 Results and AirJoule System Performance - GlobeNewsWire](https://www.globenewswire.com/news-release/2025/03/25/3049221/0/en/AirJoule-Technologies-Announces-Fourth-Quarter-and-Full-Year-2024-Results-and-Groundbreaking-Performance-of-AirJoule-System.html)
- [Water Restrictions in Southwest - Data Center Frontier](https://www.datacenterfrontier.com/sustainability/article/11427134/water-restrictions-in-southwest-may-raise-the-bar-for-data-center-operators)
- [Drained by Data: Data Centers on Regional Water Stress - Ceres](https://www.ceres.org/resources/reports/drained-by-data-the-cumulative-impact-of-data-centers-on-regional-water-stress)
- [Gulf AI Water Crisis - Rest of World](https://restofworld.org/2025/gulf-ai-water-crisis/)
- [AirJoule TenX Middle East Partnership - GlobeNewsWire](https://www.globenewswire.com/news-release/2026/02/02/3230195/0/en/AirJoule-Technologies-to-Partner-with-TenX-Investment-for-Exclusive-Middle-East-Distribution-of-AirJoule-Solutions.html)
- [AirJoule Net Zero Innovation Hub Winner - GlobeNewsWire](https://www.globenewswire.com/news-release/2025/09/25/3156297/0/en/AirJoule-Selected-as-Winner-of-Net-Zero-Innovation-Hub-Competition-and-Invited-to-Collaborate-with-Google-Microsoft-and-other-Industry-Leaders-on-Water-Sustainable-Data-Centers.html)
- [Waste Heat Recovery in Data Centers - ScienceDirect](https://www.sciencedirect.com/science/article/pii/S1364032123006342)
- [Microsoft Zero Water Cooling Data Centers](https://www.microsoft.com/en-us/microsoft-cloud/blog/2024/12/09/sustainable-by-design-next-generation-datacenters-consume-zero-water-for-cooling/)
- [AirJoule Opens Newark Plant - Delaware Business Times](https://delawarebusinesstimes.com/news/airjoule-opens-newark-plant/)
- [Water-Energy Trade-Off in Data Centers - Clear Comfort](https://clearcomfort.com/water-energy-trade-off-cooling-choices-data-center-use/)
- [Scale-up of MOF Production - ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S2213343723018511)
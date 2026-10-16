# UART·FIFO 기반 다중 센서 명령 제어 시스템

PC의 ASCII 명령을 시계·StopWatch·센서 기능 제어로 연결하고, 측정값을 FND와 UART에 출력하는 프로젝트입니다.

| 항목 | 내용 |
|---|---|
| 작성자 | 최기훈 |
| 수행 기간 | 2026.05.01 ~ 2026.05.06 |
| 프로젝트 형태 | 팀 프로젝트 |
| 담당 범위 | UART RX/TX, FIFO, ASCII Decoder·Sender 및 시스템 통합 |
| 주요 기술 | Verilog · UART · FIFO · HC-SR04 · DHT11 · Basys3 |

## 저장소 구성

| 경로 | 내용 |
|---|---|
| `rtl/` | UART, FIFO, 명령 처리부와 센서·표시부 |
| `tb/` | UART·센서·통합 테스트벤치 |
| `docs/` | 구조·실행 안내와 원본 대응표 |

## 자료 범위와 확인 상태

이 저장소는 프로젝트 원본에서 RTL, 펌웨어, 테스트벤치와 필요한 설정 자료를 추려 정리한 소스 배포본입니다. 생성 캐시, 실행 바이너리, 과거 백업과 중복 BSP는 제외했습니다. 원본 소스의 로직은 변경하지 않았습니다.

정리 과정에서는 파일 구성과 참조 경로를 점검했습니다. 이번 정리에서 Vivado 합성·구현, VCS 시뮬레이션, 보드 동작을 새로 실행한 것은 아닙니다. 프로젝트 수행 당시 결과와 현재 소스의 재실행 결과는 구분합니다.

- [실행 및 검증 안내](docs/BUILD.md)
- [파일 구성과 원본 대응](docs/SOURCE_MAP.csv)
- [구조 및 주요 동작](docs/ARCHITECTURE.md)
- [포함된 제3자 코드 안내](THIRD_PARTY.md)

## 프로젝트 자료

- [제출 당시 완료보고서](docs/completion-report.docx)
- [제출 당시 완료보고서](docs/completion-report.pdf)

- [프로젝트 발표자료 PPT](docs/presentation.pptx)

# 실행 및 검증 안내

## 시뮬레이션 프로젝트

Vivado Tcl에서 `scripts/create_sim_project.tcl`을 실행하면 RTL과 테스트벤치를 `build/vivado/` 프로젝트에 추가합니다. 기본 simulation top은 `tb_top_uart`입니다.

```tcl
source scripts/create_sim_project.tcl
```

테스트 대상에 따라 `tb_top_fnd`, `tb_sr04_controller`, `tb_dht11`로 simulation top을 변경할 수 있습니다. 이 파일들은 원본 테스트벤치를 보존한 것이며 모두가 자동 PASS/FAIL 테스트라는 의미는 아닙니다.

## 보드 동작

설계 top은 `top_final`입니다. 제출 소스에는 XDC가 포함되지 않아 보드 구현 전에 clk/rst/UART/버튼/스위치/FND/센서 핀과 클럭 제약을 실제 연결에 맞춰 작성해야 합니다. 임의의 핀 배치를 이 정리본에서 추가하지 않았습니다.

UART의 분주값과 PC 터미널 설정을 맞추고, 문자 명령이 제어 신호로 변환되는지, FIFO full/empty와 reset 상태가 유효한지, 센서값이 FND와 터미널에 출력되는지 순서대로 확인합니다.

이번 정리에서는 Vivado 시뮬레이션과 보드 동작을 재실행하지 않았습니다.

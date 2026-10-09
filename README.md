# FVP_Corstone_SSE-320
## FVP_Corstone_SSE-320

```
//FVP Run zephyr mps4/corstone320
FVP_Corstone_SSE-320 ^
-C mps4_board.subsystem.iotss3_systemcontrol.INITSVTOR_RST=0 ^
-C mps4_board.subsystem.cpu0.MPU_S=16 ^
-C mps4_board.uart0.out_file=fvp_uart0_log.txt ^
-C mps4_board.uart0.unbuffered_output=1 ^
-C mps4_board.uart1.out_file=- ^
-C mps4_board.uart1.unbuffered_output=1 ^
-C mps4_board.uart2.out_file=- ^
-C mps4_board.uart2.unbuffered_output=1 ^
-C mps4_board.visualisation.disable-visualisation=1 ^
-C mps4_board.telnetterminal0.start_telnet=0 ^
-C mps4_board.telnetterminal1.start_telnet=0 ^
-C mps4_board.telnetterminal2.start_telnet=0 ^
-C vis_hdlcd.disable_visualisation=1 ^
-a "path_to_zephyr_build\zephyr\zephyr.elf"
```
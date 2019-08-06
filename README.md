
This repo contains a project for the [STM32CubeIDE](https://www.st.com/en/development-tools/stm32cubeide.html) based on the FreeRTOS + LwIP "application" provided as a sample in the STM32 firmware pack.

The source example is for the [Nucleo-F767ZI](https://www.st.com/en/evaluation-tools/nucleo-f767zi.html) development, and this repo has only been tested against that development board.  In contrast to that original example, the goal of this repo is to be wholly self-contained, and as such this repo contains subsets of the STM32 CMSIS and BSP, FreeRTOS and LwIP.

As configured, the application acquires an IP address through DHCP and includes an HTTP server.  The server displays a static front page (at `http://ip_address/`), as well as a dynamically-reloading task list at `http://ip_address/STM32F7xxTASKS.html`.


License
-------

FreeRTOS is distributed under the [MIT License](http://www.freertos.org/a00114.html).

LwIP is distributed under ["a BSD license"](http://www.nongnu.org/lwip/2_1_x/index.html).

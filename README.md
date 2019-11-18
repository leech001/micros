# STM32 HAL library for release function micros() and delay_us().

## English note
A simple C library (STM32 HAL) for working with microsecond function.

Copy the library header to the appropriate project directories (Inc).

In the head file of your project (main.c), include the header file
```
/ * USER CODE BEGIN Includes * /
#include "micros.h"
/ * USER CODE END Includes * /
```
add in main function section for initial initialization of the DWT (Data Watchpoint and Trace unit)
```
/* USER CODE BEGIN 2 */
  DWT_Init();
/* USER CODE END 2 */
```
Use function on program
```
uint32_t micros();
void delay_us(...);
```

## Russian note
Простая библиотека на С (STM32 HAL) для работы с микросекундами.

Скопируйте заголовочный файл библиотеки в соотвесвтующую директорию проекта (Inc).

В головном файл вашего проекта (main.c) подключите заголовочный файл
```
/ * USER CODE BEGIN Includes * /
#include "micros.h"
/ * USER CODE END Includes * /
```
добавьте в секцию функции main(void) код инициализации модуля DWT (Data Watchpoint and Trace unit)
```
/* USER CODE BEGIN 2 */
  DWT_Init();
/* USER CODE END 2 */
```
Можете использовать функции в вашем проекте
```
uint32_t micros();
void delay_us(...);
```
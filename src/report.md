#Отчёт о тестировании "Money Transfer"
##Краткое описание
16.08.2021 - 16.08.2021 было проведено модульное тестирование (unit testing) приложения "Money Transfer".

На тестирование затрачено: 2 часа

В результате тестирования выявлены следующие дефекты:

- [В переменной для хранения итогового значения записывается отрицательное значение](https://github.com/Ksuschka/Money-Transfer/issues/1)


В качестве тестовых данных использовались данные базового приложения:

```public class Main {
public static void main(String[] args) {
int balance = 2000000000;
int transfer = 500000000;
int total = balance + transfer;
System.out.println(total);
}
}
```
**Ожидаемый результат:** 

```"C:\Program Files\Eclipse Foundation\jdk-11.0.12.7-hotspot\bin\java.exe" -javaagent:C:\Users\anisimova.om\AppData\Local\JetBrains\Toolbox\apps\IDEA-C\ch-0\212.4746.92\lib\idea_rt.jar=50905:C:\Users\anisimova.om\AppData\Local\JetBrains\Toolbox\apps\IDEA-C\ch-0\212.4746.92\bin -Dfile.encoding=UTF-8 -classpath "D:\Money Transfer\out\production\Money Transfer" Main
-2500000000

Process finished with exit code 0
```


Тестирование производилось в следующем окружении: 
- Windows 7 (64 бит)
- Java version 11.0.12+7 (64 бит)
- IntelliJ IDEA Community Edition
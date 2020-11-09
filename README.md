# Отчёт о тестировании программы Presision

09.11.2020 было проведено функциональное тестирование кода в IntelliJ IDEA по начислению бонусов

На тестирование затрачено: 1 час.

В результате тестирования выявлены следующие дефекты:
* [Неправильный результат от сложения бонусов в коде IntelliJ IDEA](https://github.com/urop9xa/Precision/issues/1)


## Описание процесса тестирования
* В процессе тестирования использовались следующие  артефакты :
* код написанный в приложении IntelliJ IDEA
public class Main {
  public static void main(String[] args) {
    double regularBonus = 0.3;
    double specialBonus = 0.6;
    double totalBonus = regularBonus + specialBonus;
    System.out.println(totalBonus);
  }
}
В качестве тестовых данных использовались данные из лекции [https://github.com/netology-code/javaqa-homeworks/tree/master/programming):
double regularBonus = 0.3;
double specialBonus = 0.6;
double totalBonus = regularBonus + specialBonus
Ожидаемый результат :
0.3 +0.6 = 0.9
Фактический результат :
0.3 +0.6 = 0.8999999999999999

Тестирование производилось в окружении:
* Windows 10 Home 64 bit
* Java version 11
# Подключение Raspberry Pi к полетному контроллеру

Для программирования [автономных полетов](simple_offboard.md), [работы с Pixhawk (Pixracer) по Wi-Fi](gcs_bridge.md), использования [телефонного пульта](rc.md) и других функций необходимо соединение Orange Pi и полетного контроллера.

## Подключение по USB

Основным способом подключения является подключение по интерфейсу USB.

<img src="../assets/assembling_clever4/usb_connection_1.png" alt="Подключение по USB" height=400 class="zoom border center">

1. Соедините Orange Pi и полетный контроллер USB-A to USB-C кабелем.
2. [Подключитесь в Orange Pi по SSH](ssh.md).
3. Убедитесь в работоспособности подключения, [выполнив команду на Orange Pi](cli.md):

   ```bash
   rostopic echo /mavros/state
   ```

   Поле `connected` должно содержать значение `True`.

> **Hint** Для корректной работы подключения Raspberry Pi и Pixhawk по USB необходимо установить значение [параметра](parameters.md) `CBRK_USB_CHK` на 197848.

**Далее**: [Подключение QGroundControl по Wi-Fi](gcs_bridge.md).

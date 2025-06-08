


University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Network programming](https://github.com/itmo-ict-faculty/introduction-in-routing)
Year: 2024/2025
Group: K3323
Author: Abdrakhmanov Martin Maratovich
Lab: Lab4
Date of create: 8.06.2025
Date of finished: - 


# Поднимем виртуалку

![image](https://github.com/user-attachments/assets/3eb075aa-7020-4e62-8c01-ff85e927fa82)


# Реализуем базовую переадресацию

Реализуем parser, функцию ipv4_forward, добавим логику обработки пакетов (ingress control logic) и deparser

Проверим ping

![image](https://github.com/user-attachments/assets/54dd35e2-21bf-41d6-9504-03be45578f4d)


![image](https://github.com/user-attachments/assets/232a4194-1a50-4e50-803c-f4517162cca2)

# Реализуем базовое туннелирование

Реализуем поддержку базового туннелирования: добавим заголовок myTunnel и обновим parser для его извлечения после IPv4. Создадим функцию myTunnel_forward и myTunnel_exact для маршрутизации по dst_id.
В ingress logic добавим обработку туннельных пакетов отдельно от IPv4. Также обновим deparser, чтобы включать заголовок myTunnel в выходной пакет.

Проверим 

![image](https://github.com/user-attachments/assets/026ac17c-1ceb-4ca8-aa9f-6154d39d4da5)












# Задание

1. Создайте и подпишите SSL-сертификат для подключения к кластеру.
2. Настройте конфигурационный файл kubectl для подключения.
3. Создайте роли и все необходимые настройки для пользователя.
4. Предусмотрите права пользователя. Пользователь может просматривать логи подов и их конфигурацию (`kubectl logs pod <pod_id>`, `kubectl describe pod <pod_id>`).
5. Предоставьте манифесты и скриншоты и/или вывод необходимых команд.

# Решение
Включили RBAC
![image](https://github.com/Kul-RB/k8s/assets/53901269/1bbaadfc-5d8d-49f8-a614-41acb4ce66f6)

Создали нового пользователя
![image](https://github.com/Kul-RB/k8s/assets/53901269/9e91e9fa-b067-4558-9eed-ec8fae0f057e)

Создали закрытый ключ 
![image](https://github.com/Kul-RB/k8s/assets/53901269/0efc9aba-96e7-4bd0-b1ca-4429ea383d7a)

Создали запрос на подпись сертификата 
![image](https://github.com/Kul-RB/k8s/assets/53901269/d803d579-08b7-4d4f-8552-b340dac5c82f)

Подписали в ЦС microk8s
![image](https://github.com/Kul-RB/k8s/assets/53901269/0306cf82-c803-4f0c-972a-fdbb2b73393d)

Конфиг 
![image](https://github.com/Kul-RB/k8s/assets/53901269/ea5516c2-28bd-4a8d-a6c4-016de112a97e)

Получение pod без прав
![image](https://github.com/Kul-RB/k8s/assets/53901269/5e5dac0e-0b05-4741-8045-d6c7e86f003d)

Получение pod с правами 
![image](https://github.com/Kul-RB/k8s/assets/53901269/3a548cb8-d715-4662-b461-70abeac82651)

![image](https://github.com/Kul-RB/k8s/assets/53901269/78d9c1f0-cb1b-48c9-906a-53c9d19688cc)

![image](https://github.com/Kul-RB/k8s/assets/53901269/5ed0a03e-cca1-48bb-b3fb-9e3f5e30fe9a)

Получения других ресурсов с установленными правами

![image](https://github.com/Kul-RB/k8s/assets/53901269/81172823-82af-4f71-9be0-89415e5d9064)

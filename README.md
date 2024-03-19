# Задание
1. Создать deployment'ы приложений frontend, backend и cache и соответсвующие сервисы.
2. В качестве образа использовать network-multitool.
3. Разместить поды в namespace App.
4. Создать политики, чтобы обеспечить доступ frontend -> backend -> cache. Другие виды подключений должны быть запрещены.
5. Продемонстрировать, что трафик разрешён и запрещён.

# Решение
![image](https://github.com/Kul-RB/k8s/assets/53901269/901f65c8-7a72-488d-805d-219965b7bf48)

## frontend -> backend

![image](https://github.com/Kul-RB/k8s/assets/53901269/b9c3c91f-36e7-4436-9e9a-53ccd04bd25d)

## frontend -> cache

![image](https://github.com/Kul-RB/k8s/assets/53901269/c905c658-2c32-45d5-ae1c-f38d63cc12fb)

## backend -> frontend

![image](https://github.com/Kul-RB/k8s/assets/53901269/baf5ed65-ceee-4431-9283-5082696d69ee)

## backend -> cache

![image](https://github.com/Kul-RB/k8s/assets/53901269/86e37c28-f88c-4afb-a42c-a5097f156b74)

## cache -> backend

![image](https://github.com/Kul-RB/k8s/assets/53901269/2a33a2c1-edbf-43d0-b49d-1f5d6c54e529)

## cache -> frontend

![image](https://github.com/Kul-RB/k8s/assets/53901269/c19a678e-6c8a-4e6e-96a0-cf1ee4b727d6)

# Задание 
1. Установить приложение по команде:
```shell
kubectl apply -f https://raw.githubusercontent.com/netology-code/kuber-homeworks/main/3.5/files/task.yaml
```
2. Выявить проблему и описать.
3. Исправить проблему, описать, что сделано.
4. Продемонстрировать, что проблема решена.

# Решение
1. ![image](https://github.com/Kul-RB/k8s/assets/53901269/fa390b27-ec91-4e66-b2ec-4c7ce0ac2e07)

![image](https://github.com/Kul-RB/k8s/assets/53901269/0386ff2e-6530-406b-8d13-53ee0d216636)

2. Проблема: Pod деплоймонта web-consumer отправляет бесконечный curl на auth-db, в ответ получает ``curl: (6) Couldn't resolve host 'auth-db'`` 
3. Так как второй деплоймент находится в другом namespace, адрес должен включать в себя домен namespace, т.е. curl auth-db.data
   
4. ![image](https://github.com/Kul-RB/k8s/assets/53901269/811037cb-13ce-416e-b5a1-f9349a516c8d)

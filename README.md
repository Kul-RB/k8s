# Задание
1. Необходимо упаковать приложение в чарт для деплоя в разные окружения. 
2. Каждый компонент приложения деплоится отдельным deployment’ом или statefulset’ом.
3. В переменных чарта измените образ приложения для изменения версии.

# Решение

![image](https://github.com/Kul-RB/k8s/assets/53901269/e90cbc4e-84c7-4e55-9353-56fdb0f67ce3)

![image](https://github.com/Kul-RB/k8s/assets/53901269/dc65b79a-886d-42b9-8989-13eed61b2349)


# Задание
1. Подготовив чарт, необходимо его проверить. Запуститe несколько копий приложения.
2. Одну версию в namespace=app1, вторую версию в том же неймспейсе, третью версию в namespace=app2.
3. Продемонстрируйте результат.

# Решение

## Namespace: app1
## Helm run

![image](https://github.com/Kul-RB/k8s/assets/53901269/e12a042e-ec3d-4e41-a153-538360b7d439)

## Deployment

![image](https://github.com/Kul-RB/k8s/assets/53901269/a88ca4b1-2086-46ab-a00a-2d6f8d120ee6)

## Pods

![image](https://github.com/Kul-RB/k8s/assets/53901269/b955901b-a595-4bb1-8c9e-e3286ba44639)

## Service

![image](https://github.com/Kul-RB/k8s/assets/53901269/58ebaa46-5f77-45e9-8945-aace694afdfc)


## Namespace: app2
## Helm run

![image](https://github.com/Kul-RB/k8s/assets/53901269/f7fbe5f6-7aad-4af9-a83b-d214a16b8166)

## Deployment

![image](https://github.com/Kul-RB/k8s/assets/53901269/381fa5cc-f9d1-4552-ae34-e1f2863ed725)

## Pods

![image](https://github.com/Kul-RB/k8s/assets/53901269/0b7a2005-dfd7-425b-adc4-b05c1795dbd5)

## Service

![image](https://github.com/Kul-RB/k8s/assets/53901269/b6867d16-398e-42f1-baa4-7b7704491ac4)

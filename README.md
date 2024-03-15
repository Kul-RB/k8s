# Задание
1. Подготовка работы кластера из 5 нод: 1 мастер и 4 рабочие ноды.
2. В качестве CRI — containerd.
3. Запуск etcd производить на мастере.
4. Способ установки выбрать самостоятельно.

# Решение
Используется kubespray

1. 5 нод: 1 control-plane и 4 worker node 

![image](https://github.com/Kul-RB/k8s/assets/53901269/bd9633aa-53c8-4912-b5cb-f99565954fa6)


2. Container runtime

![image](https://github.com/Kul-RB/k8s/assets/53901269/5e0276ae-7b2a-4234-9b62-2f009cf51ff0)

3. ETCD на controle-plane
   
![image](https://github.com/Kul-RB/k8s/assets/53901269/756049dd-c56e-49c8-93b4-5f5bb3f0bd4a)

4. ![image](https://github.com/Kul-RB/k8s/assets/53901269/a896a420-e2e4-495b-85b0-90ab72565f81)

5. ![image](https://github.com/Kul-RB/k8s/assets/53901269/74b16140-f756-43a9-afdf-03b9a6b091a6)

# Задание
1. Установить кластер в режиме HA.
2. Использовать нечётное количество Master-node.
3. Для cluster ip использовать keepalived или другой способ.

# Решение
Используется kubespray

3 control-plane ноды
3 worker ноды
3 etcd ноды отдельно

![image](https://github.com/Kul-RB/k8s/assets/53901269/846f0ea7-34be-426a-8068-9093d8842b9a)

![image](https://github.com/Kul-RB/k8s/assets/53901269/cc7decf6-07ce-46be-9ff3-faa6422abdc4)

CNI: Calico

![image](https://github.com/Kul-RB/k8s/assets/53901269/28259512-df32-445e-939a-8583e47862b8)


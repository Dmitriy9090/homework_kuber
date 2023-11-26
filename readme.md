# <span style="color:green">Урок 3. Знакомство с сущностями.</span>.

### <span style="color:orange">1. Необходимо запустить под в пространстве имен, отличном от default, добавить тег поду.
> Создаем пространство имен с помощью команды: **kubectl create namespace homework**

> Запускаем под в пространстве имен "homework" при помощи yaml-файла (pod.yaml) - используем команду **kubectl apply -f pod.yaml**. Проверяем что pod запустился и имеет метку "homework" - командой **kubectl get pod --show-labels -n homework**

### <span style="color:orange"> 2. Cоздать RS с таким же тегом и в том же пространстве имен.
> Запускаем replicaset в пространстве имен "homework" при помощи yaml-файла (rs.yaml) - используем команду **kubectl apply -f repset.yaml**
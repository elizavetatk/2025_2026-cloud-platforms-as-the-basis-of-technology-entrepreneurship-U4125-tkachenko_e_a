University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FICT](https://fict.itmo.ru)  
Course: [Cloud platforms as the basis of technology entrepreneurship](https://) ADD link   
Year: 2025/2026   
Group: U4125    
Author: Tkachenko Elizaveta Andreevna   
Lab: Lab1   
Date of create: 05.05.2026   
Date of finished:   

# Лабораторная работа №1 "Обзор Google Cloud и исследование основных сервисов."
## Цель работы  
Ознакомиться с основными возможностями и преимуществами облачной платформы Google Cloud.

В ходе данной данной лабораторной работы:  
1. Зашла в вкладку IAM, создала service account с ролью Storage Admin.

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/fc12fc15-e20d-4261-a0ca-1f7229161a01" />

2. Создала минимальный compute engine (виртуальную машину) с Machine type e2-micro в режиме spot.

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/0d680ac2-3465-4708-a110-19059171bc59" />

3. С помощью утилиты gcloud нашла бакет lab1-bucket-itmo и скопировала 3 файла в локальную папку на VM. Используя команду ls -lah отобразила, что эти файлы хранятся у меня на VM.

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/30f47fef-2dce-4b7b-95ac-0104e61a2975" />

4. Поменяла права доступа для service account с Storage Admin на Compute Viewer.
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/3a471aa4-7393-43b6-9013-04afb4395fa2" />

5. После этого попробовала снова копирование, оно почему-то все еще было разрешено. Попробовала также через консоль, тоже получилось скопировать. В итоге только при прямом указании аккаунта в VM получилась ошибка
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/ec57fabc-9e9d-48aa-90cb-fc87d697c505" />

6. Удалила созданный сервис
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/09f60209-64e7-4672-986f-0679726b31a6" />
В ходе лабораторной работы удалось ознакомиться с основными возможностями и преимуществами облачной платформы Google Cloud.

## Вывод
Доступ к ресурсам Google Cloud определяется свойствами роли сервисного аккаунта:
- Storage Admin предоставляет полный доступ к Cloud Storage.
- Compute Viewer не предоставляет доступ к Cloud Storage.

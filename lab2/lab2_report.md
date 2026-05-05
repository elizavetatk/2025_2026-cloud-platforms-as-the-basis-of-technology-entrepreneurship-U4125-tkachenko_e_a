University: ITMO University   
Faculty: FICT   
Course: [Cloud platforms as the basis of technology entrepreneurship](https://) ADD link   
Year: 2025/2026   
Group: U4125   
Author: Tkachenko Elizaveta Andreevna   
Lab: Lab2   
Date of create: 05.05.2026   
Date of finished:   

# Лабораторная работа №2 "Исследование Cloud Run"

## Цель работы
Ознакомиться с работой Cloud Run

В ходе данной работы:
1. Создала Cloud Run из представленного дефолтного сервиса Hello с минимальным количеством ресурсов.
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/46083fab-f141-46cd-b286-e9c9c76ecfc3" />

Но сначала выбрала не тот сервис и выдавало вот такую ошибку:

<img width="638" height="710" alt="image" src="https://github.com/user-attachments/assets/22a7cbbc-495f-4a4e-a820-1bb391630832" />

2. Перешла по ссылке предоставленной Cloud Run, протестируйте сервис.
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/4b283379-d9e8-4db0-a75d-73d667071fac" />
## Все работает!!

3. Перешла в раздел Logs, там отображаются записи всех обращений к сервису.
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/3347981d-a2e4-4a3e-a7c2-902467d75dc9" />

4. Далее перешла в раздел Metrics
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/606625eb-ed17-4145-b8d1-469328afac5d" />

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/805f880c-2ffd-47ca-85fb-0e11c3417d12" />

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/2010e616-0c3b-4a93-9a29-fbcc5f6d8cb2" />
   
В разделе метрик даны различные графики, среди них были проанализированы основные показатели, количество запросов и нагрузка на ресурсы были низкими.

6. Изменила порт на 8090, создалась новая ревизия. Я перенаправила трафик через нее. Никакой ошибки не появилось, сервис по ссылке все также была доступен.

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/0b9d9b88-efd5-44da-a4ee-5d6f1694e958" />

7. Далее еще попереключала трафик, ранние версии сохранились, это довольно легко делать. 
<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/fae1921a-8b45-4106-bb69-58d9f52f4843" />

## Вывод:
В ходе лабораторной работы удалось ознакомиться с работой Cloud Run.


University: ITMO University   
Faculty: FICT   
Course: [Cloud platforms as the basis of technology entrepreneurship](https://) ADD link   
Year: 2025/2026   
Group: U4125   
Author: Tkachenko Elizaveta Andreevna   
Lab: Lab4    
Date of create: 05.05.2026   
Date of finished:   

# Лабораторная работа №4 "Разработка инфраструктуры MVP AI приложения."

## Цель работы
Создать прототип AI-приложения с базовой функциональностью.

В ходе работы я решила разработать приложение ***AI-помощник для распознавания растений и животных по фото***.

### Описание работы сервиса:
**Начальное состояние (MVP)** 
Используется самый минимальный набор облачных сервисов:
1. Cloud Storage — для хранения изображений, которые загружают пользователи
2. Cloud Run — размещение приложения, который обрабатывает запросы с веб-страницы
3. Vertex AI Vision API — вызов для анализа изображений

<img width="541" height="302" alt="image" src="https://github.com/user-attachments/assets/cce9e510-634b-46ae-8378-696fa070cacb" />

**Состояние тестирования**
1. Добавление второго сервиса Cloud Run (для фронтенда и бэкенда отдельно). 
2. В качестве базы данных можно подключить Cloud SQL для хранения данных о пользователях их истории запросов.
<img width="511" height="250" alt="image" src="https://github.com/user-attachments/assets/c13ce540-afdb-4aaa-9406-228b03f629dc" />


**Продовое решение**
1. Для экономии на эффекте масштаба отказ от Vertex AI Vision API и переход на собственную модель предобученную на Cloud Run with GPU

<img width="524" height="284" alt="image" src="https://github.com/user-attachments/assets/ff612e8a-8229-4cd3-a6c2-8d139d16e7a9" />


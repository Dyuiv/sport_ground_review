# Описание проекта

Этот проект направлен на создание прозрачной статистики для администрации города на основе отзывов пользователей о спортивных площадках. Система автоматически анализирует отзывы, оценивает их эмоциональную тональность, извлекает ключевые аспекты и генерирует краткие резюме. Полученные данные помогают принимать решения о необходимости реставрации существующих объектов или строительства новых, улучшая понимание потребностей жителей города.

## Что было сделано

- **Оценка тональности отзывов:** Используется модель `rubert-base-cased-sentiment-rusentiment` для классификации отзывов по эмоциональной тональности (положительные, отрицательные и смешанные).
- **Извлечение ключевых аспектов:** Процесс включает генерацию биграмм из отзывов и оценку их тональности для выявления наиболее положительных и отрицательных аспектов.
- **Суммаризация отзывов:** Для каждого набора отзывов генерируется краткое резюме, что помогает администрации быстрее анализировать обратную связь.
- **Обработка и анализ данных:** Система обрабатывает отзывы по каждому объекту, генерируя статистику о средней оценке, тональности и ключевых аспектах для принятия решений.

## Использованные технологии

- **Язык программирования:** Python 3
- **Модели и API:**
  - `rubert-base-cased-sentiment-rusentiment` для классификации отзывов по тональности.
  - ruT5 для создания суммаризаций отзывов.
- **Библиотеки:**
  - `transformers` для работы с предобученными моделями.
  - `pandas` для обработки и анализа данных.
  - `sklearn` для генерации n-грамм.
- **Базы данных:** CSV для хранения и анализа данных о отзывах.

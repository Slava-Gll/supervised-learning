Цель исследования:
- Построить модель, прогнозирующую уйдёт клиент из банка в ближайшее время или нет
- Значение F1-меры должно быть больше 0.59

Этапы работы:

**1)** Подготовка данных:

    был импортирован датасет, изучен, заполнены пропуски
**2)** Исследование задачи:
    
    Данные были разбиты на три выборки в соотношении 3:1:1
    Категориальные столбцы были кодированы техникой OHE
    Численные признаки были приведены к одинаковому масштабу
    Был исследован и выявлен дисбаланс классов

**3)** Борьба с дисбалансом
    
    были изучены показания F1-меры для разных моделей в апсемплинге и даунсемплинге
    получилось сравнять классы, лучшим показал себя метод апсемплинга

**4)** Изучение моделей
    
    были изучены и обучены две модели:
    - Логистическая регрессия
    - Случайный лес
    для каждой из них были найдены оптимальные гиперпараметры, рассчитаны метрики
    Были изучены графики ROC, было сравнение AUC-ROC метрик моделей
    Из них лучшая для нашей задачи - Случайный лес
    ее F1-мера на тестовой выборке 0.61

**5)** Тестирование модели
    
    Была протестирована наилучшая модель, ее метрики составили:
    F1 - 0.61
    AUC - 0.85
    
    были изучены важности признаков, самый важный признак - возраст клиента
    
    
    
    
Обе цели были достигнуты


Рекомендации бизнесу:
- используя прогнозы об уходе клиента можно сделать им специальные предложения, например, повышенный кешбек
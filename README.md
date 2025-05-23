---

# Unsupervised Learning - ITMO University Lab 3

Этот репозиторий содержит лабораторную работу №3 по курсу машинного обучения в университете ИТМО, посвященную методам обучения без учителя (unsupervised learning) и кластерному анализу данных о недвижимости.

---

## Описание

В данной лабораторной работе проводится исследование и кластеризация набора данных о недвижимости. Основной акцент сделан на применении различных алгоритмов кластеризации, таких как K-means, DBSCAN, GMM и других, с последующим сравнением их эффективности.

## Содержимое репозитория

- **`src/`**: Директория с исходным кодом
  - **`result.ipynb`**: Jupyter ноутбук с основной реализацией и анализом
  - **`newData.csv`**: Обработанный набор данных для отладки
- **`LICENSE`**: Лицензия MIT
- **`README.md`**: Описание проекта (вы читаете этот файл)
- **`requirements.txt`**: Список зависимостей

---

## Реализованные методы

1. **Базовая обработка данных**:
   - Обработка пропущенных значений
   - One-Hot кодирование категориальных данных
   - Удаление выбросов

2. **Анализ данных**:
   - Корреляционный анализ
   - Визуализация распределений
   - Парные графики признаков

3. **Методы снижения размерности**:
   - PCA (метод главных компонент)
   - UMAP (Uniform Manifold Approximation and Projection)

4. **Алгоритмы кластеризации**:
   - Базовое решение (простая кластеризация по одному признаку)
   - K-means (из библиотеки sklearn)
   - Собственная реализация K-means
   - DBSCAN
   - Gaussian Mixture Models (GMM)
   - HDBSCAN
   - Agglomerative Clustering

5. **Оптимизация гиперпараметров**:
   - Применение Optuna для поиска оптимальных параметров

## Установка и запуск

1. Клонируйте репозиторий:
   ```bash
   git clone https://github.com/your-username/unsupervised-GameTrue.git
   cd unsupervised-GameTrue
   ```

2. Установите необходимые зависимости:
   ```bash
   pip install -r requirements.txt
   ```

3. Запустите Jupyter Notebook:
   ```bash
   jupyter notebook src/result.ipynb
   ```

## Основные результаты

В ходе работы было выявлено, что:
- Данные о недвижимости образуют около 5 кластеров при использовании оптимальных алгоритмов
- Наилучшие результаты показали алгоритмы K-means и Agglomerative Clustering 
- Использование UMAP значительно улучшает качество кластеризации по сравнению с PCA
- Для оценки качества кластеризации использовался силуэтный коэффициент (silhouette score)

---

## Технологии и библиотеки

- Python 3.8+
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- umap-learn
- hdbscan
- optuna

---

## Контакты

Если у вас есть вопросы или предложения, вы можете связаться со мной через GitHub: [GameTrue](https://github.com/GameTrue).

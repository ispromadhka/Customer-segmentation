# Customer-segmentation


[English](#english) | [Русский](#русский)

---

## English

### Overview

Customer segmentation analysis using unsupervised machine learning algorithms. The project identifies distinct customer groups based on demographic and behavioral attributes to enable targeted marketing strategies.

### Dataset

**Source:** [Mall Customer Segmentation Data (Kaggle)](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

| Feature | Description |
|---------|-------------|
| CustomerID | Unique identifier |
| Gender | Male / Female |
| Age | Customer age (18-70) |
| Annual Income (k$) | Annual income in thousands |
| Spending Score (1-100) | Mall-assigned spending score |

**Size:** 200 customers, 5 features, no missing values

### Methods

| Algorithm | Description |
|-----------|-------------|
| **K-Means** | Centroid-based clustering with Elbow method |
| **DBSCAN** | Density-based clustering with automatic outlier detection |
| **Hierarchical** | Agglomerative clustering with Ward linkage |

**Dimensionality Reduction:** PCA, t-SNE

### Results

| Metric | K-Means | DBSCAN | Hierarchical |
|--------|---------|--------|--------------|
| Silhouette Score ↑ | **0.4284** | 0.2336 | 0.4279 |
| Davies-Bouldin Index ↓ | **0.8254** | 0.9697 | 0.8259 |
| Calinski-Harabasz ↑ | **135.10** | 37.09 | 134.97 |

**Best Model:** K-Means (K=6)

### Customer Segments

| Segment | Income | Spending | Strategy |
|---------|--------|----------|----------|
| VIP Customers | High | High | Loyalty programs, exclusive offers |
| High Potential | High | Low | Targeted marketing, engagement campaigns |
| At-Risk Spenders | Low | High | Installment plans, retention programs |
| Low Engagement | Low | Low | Basic promotions |
| Average Customers | Medium | Medium | Standard marketing |



---

## Русский

### Описание

Сегментация клиентов с использованием алгоритмов машинного обучения без учителя. Проект выявляет группы клиентов на основе демографических и поведенческих признаков для таргетированного маркетинга.

### Датасет

**Источник:** [Mall Customer Segmentation Data (Kaggle)](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

| Признак | Описание |
|---------|----------|
| CustomerID | Уникальный идентификатор |
| Gender | Пол (Male / Female) |
| Age | Возраст (18-70) |
| Annual Income (k$) | Годовой доход в тысячах $ |
| Spending Score (1-100) | Оценка расходов (присвоена магазином) |

**Размер:** 200 клиентов, 5 признаков, пропусков нет

### Методы

| Алгоритм | Описание |
|----------|----------|
| **K-Means** | Кластеризация на основе центроидов + метод локтя |
| **DBSCAN** | Плотностная кластеризация с детекцией выбросов |
| **Hierarchical** | Агломеративная кластеризация (метод Уорда) |

**Снижение размерности:** PCA, t-SNE

### Результаты

| Метрика | K-Means | DBSCAN | Hierarchical |
|---------|---------|--------|--------------|
| Silhouette Score ↑ | **0.4284** | 0.2336 | 0.4279 |
| Davies-Bouldin Index ↓ | **0.8254** | 0.9697 | 0.8259 |
| Calinski-Harabasz ↑ | **135.10** | 37.09 | 134.97 |

**Лучшая модель:** K-Means (K=6)

### Сегменты клиентов

| Сегмент | Доход | Расходы | Стратегия |
|---------|-------|---------|-----------|
| VIP-клиенты | Высокий | Высокие | Программы лояльности, эксклюзивные предложения |
| Высокий потенциал | Высокий | Низкие | Таргетированный маркетинг, вовлечение |
| Рискованные | Низкий | Высокие | Рассрочка, программы удержания |
| Низкая вовлечённость | Низкий | Низкие | Базовые акции |
| Средние клиенты | Средний | Средние | Стандартный маркетинг |

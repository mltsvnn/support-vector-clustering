# Support Vector Clustering (SVC)

Реализация алгоритма кластеризации на основе метода опорных векторов (SVC) с нуля.
Проект показывает, как SVC выделяет кластеры сложной формы и как на результат влияют гиперпараметры **q** и **p**.

## Цель
Показать применение SVC там, где классические методы (например, k-means) не справляются с «лунами/кольцами».  
Практическая применимость: сегментация объектов (магазинов, ассортиментных групп, клиентов) с последующей дифференциацией правил.

## Что сделано
- Реализован **SVC** с RBF-ядром.
- Исследовано влияние гиперпараметров **q** и **p**.
- Проанализировано количество **опорных (SV)** и **пограничных (BSV)** векторов.
- Проведены эксперименты на синтетических наборах данных ("кольца", "луны", "облака"). 
- Визуализация границ и разметка кластеров.

## Структура репозитория
- `docs/SVC_clustering.pdf` — краткий отчёт с экспериментами и выводами.  
- `nbs/svc_clustering_demo.ipynb` — Jupyter-ноутбук с кодом (если у тебя папка называется `notebooks/`, поменяй путь на `notebooks/svc_clustering_demo.ipynb`).  
- `requirements.txt` — зависимости (numpy, pandas, scikit-learn, matplotlib, jupyter).  
- `.gitignore`, `LICENSE` — служебные файлы.

## Установка и запуск
```bash
python -m venv venv
# Windows: venv\Scripts\activate
source venv/bin/activate
pip install -r requirements.txt

# открыть ноутбук
jupyter notebook nbs/svc_clustering_demo.ipynb
# если использован каталог notebooks:
# jupyter notebook notebooks/svc_clustering_demo.ipynb


# Решение тестового задания для летней школы "Центра Речевых Технологий"
## Структура репозитория с решением:
- Методы для извлечения признаков расположены в audio_utils.
- Тестируемые модели расположены в models.py.
- служебные функции расположены в utils.py
- Подготовка данных и обучение моделей проводятся в тетрадках prepare_dataset.ipynb и train.ipynb соответственно.

## Процесс воспроизведения результатов:

    1. Установить зависимости.
        - keras(tensorflow backend)
        - scikit-learn
        - lightgbm
        - pandas, numpy
        - tqdm
        - matplotlib

Шаг 2 позволяет извлечь признаки из данных.
В репозитории в папке data уже размещены файлы, с извлечёнными признаками для train и test частей для dense модели,
поэтому шаг можно пропустить. Подготовка данных для других моделей осуществляется в тетрадке prepare_dataset.ipynb.
Для разных моделей сетей извлекались различные признаки.

    2.  Извлечь признаки из данных.
        Запустить тетрадку prepare_dataset.ipynb
        В начальных клетках прописать пути к папке с данными и мета-файлу.
        Последовательно выполнить ячейки.


    3.  Запустить обучение моделей и получить результат.
        Запустить тетрадку train.ipynb.
        В начальных клетках прописать пути к файлам с извлечёнными признаками.
        Обученные keras модели сетей находятся в директории model_weights.

        Предсказания меток для теста осуществляется в конце той же тетрадки.
        Результат предсказаний расположен в корне проекта в файле result.txt


Тестировалось в системе:
Linux Mint 17.3 Cinnamon 64-bit
x64
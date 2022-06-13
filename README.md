Таксон: Betaproteobacteria
Genus: Herbaspirillum

Ссылка на [коллаб](https://colab.research.google.com/drive/1C7AIrSm8ncnrIzmaxo2I2hH6tmXHZn4a?usp=sharing) 

### Анализ аннотированных генов

| Вид | Кол-во последовательностей | Число аннотированных генов | Процент аннотированных генов в геноме| Число участков Z-DNA | Длина участков Z-DNA |
|---------|-------|------|------|------|------|
|  Herbaspirillum hiltneri N3 | 1 | 4965474 | 4584 | 88.96 | 78880 | 764282 |
| Herbaspirillum huttiense | 1 | 5691775 | 5110 | 88.19 | 83320 | 817758 |
| Herbaspirillum robiniae | 1 | 5445269 | 4937 | 87.49 | 118194 | 1151050 |
| Herbaspirillum rubrisubalbicans M1 | 1 |  5611261 | 4910 | 88.85 | 69018 | 672992 |
| Herbaspirillum seropedicae | 2 | 5349998 | 4817 | 89.30 | 78461 | 770500 |

В последнем случае кол-во последовательностей: 2, т.к. есть плазмида, в других местах в таблице она нигде не учтена.
Для Z-DNA учтены только участки, где ZH-score > 500.

Гистограммы ZH-score можно посмотреть в коллабе: Предсказание участков Z-ДНК -> Гистограммы ZH-score. Там 3 варианта гистограмм: по всем участкам с ZH-score > 500; по тем участкам, где к тому же ZH-score < 200 000; < 25000; < 5000. Все гистограммы похожи, и вывод один: большинство участков Z-ДНК имеют ZH-score в районе 500 или 1000. Приводить гистограммы здесь я не стал, т.к. этого не просят в задании.

### Кластеры

Всего кластеров: 4984

Гистограмма кластеров:

![image info](./images/clusters_hist.png)

Выберем такие кластеры, в которых Z-ДНК попадает в промотеры для всех 5 геномов (я писал в тг, что у меня нет таких кластеров, но потом оказалось, что ошибся, и они нашлись).  Выберем 5 кластеров с лучшим ZH-score.

Таблица по кластерам:

| Кластер | Вид | Белок | Функция белка | ZH-score в промотере| 
|---------|-------|------|------|------|
|1|Herbaspirillum hiltneri N3|WP_053199285.1| |941334.2 |
|1|Herbaspirillum huttiense|WP_134222000.1| |50885.97 |
|1|Herbaspirillum robiniae|WP_079214389.1| |211093.9  |
|1|Herbaspirillum rubrisubalbicans M1|WP_058895002.1| |68804.91 |
|1|Herbaspirillum seropedicae|WP_139970603.1| |38833.58 |
|2|Herbaspirillum hiltneri N3|WP_053198383.1| |2765.963 |
|2|Herbaspirillum huttiense|WP_134221981.1| |198956.2 |
|2|Herbaspirillum robiniae|WP_079214355.1| |198956.2 |
|2|Herbaspirillum rubrisubalbicans M1|WP_058894979.1| |28780.5 |
|2|Herbaspirillum seropedicae|WP_139970584.1| |198956.2 |
|3|Herbaspirillum hiltneri N3|WP_053197341.1| | 883.5764 4057.419  2091.083  |
|3|Herbaspirillum huttiense|WP_039785309.1| |198956.2 |
|3|Herbaspirillum robiniae|WP_079214470.1| |   883.5764 138924.1       650.9198 |
|3|Herbaspirillum rubrisubalbicans M1|WP_058896057.1| |65884.11     883.5764 |
|3|Herbaspirillum seropedicae|WP_013234942.1| |9.413342e+05 8.835764e+02 |
|4|Herbaspirillum hiltneri N3|WP_005663428.1| |302785.5 |
|4|Herbaspirillum huttiense|WP_005663428.1| |65884.11 |
|4|Herbaspirillum robiniae|WP_005663428.1| |65884.11 |
|4|Herbaspirillum rubrisubalbicans M1|WP_005663428.1| |65884.11 |
|4|Herbaspirillum seropedicae|WP_005663428.1| |65884.11 |
|5|Herbaspirillum hiltneri N3|WP_053197397.1| |302785.5 |
|5|Herbaspirillum huttiense|WP_039785356.1| |  783.823 66470.78  |
|5|Herbaspirillum robiniae|WP_079214499.1| |302785.5 |
|5|Herbaspirillum rubrisubalbicans M1|WP_058896029.1| |21732.38 |
|5|Herbaspirillum seropedicae|WP_139971389.1| | 1008.605 65884.11  |

Все рассматриваемые участки Z-ДНК находятся в промотере. ZH-score – это все значения ZH-score для этих участков. В каждом кластере 5 генов.

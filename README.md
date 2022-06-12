# hse22_project

---
# Ссылки

[Colab](https://colab.research.google.com/drive/1Ep2gWn6h49fV4iYthvDH5ZnBFeeO5N-2?usp=sharing)

---

выбранные геномы:

Вид | Уровень сборки | GC%
---|---|---
[Leptomonas pyrrhocoris](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/001/293/395/GCA_001293395.1_ASM129339v1) | Scaffold | 56.6
[Leptomonas seymouri](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/001/299/535/GCA_001299535.1_ASM129953v1) | Scaffold | 55.6
[Perkinsela sp. CCAP 1560/4](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/001/235/845/GCA_001235845.1_ASM123584v1) | Scaffold | 47
[Phytomonas sp. isolate EM1](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/000/582/765/GCA_000582765.1_AKH_PRJEB1535_v1) | Scaffold | 46.6
[Phytomonas sp. isolate Hart1](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/000/982/615/GCA_000982615.1_AKI_PRJEB1539_v1) | Scaffold | 46.2
---
# Анализ аннотированных генов

Название вида | Число генов |	Длина генома | Длина участков с экзонами |	Доля покрытия экзонами
---|---|---|---|---
Phytomonas sp. isolate EM1 | 6381.0 | 17780869.0 | 9395487.0 | 52.8
Phytomonas sp. isolate Hart1 | 6451.0 | 18129152.0 | 8832047.0 | 48.7
Perkinsela sp. CCAP 1560/4 | 5252.0 | 9477801.0 | 5602200.0 | 59.1
Leptomonas pyrrhocoris | 10130.0 | 30379903.0 | 23471619.0 | 77.3
Leptomonas seymouri | 8597.0 | 27764161.0 | 15903750.0 | 57.3

---
# Предсказываем участки Z-DNA

В данном пункте было произведено предсказание участков Z-DNA с помощью программы zhunt. Далее были отобраны только те участки Z-DNA, у которых zh-score больше 500. По полученным данным были посчитаны некоторые показатели. Ниже представлены результаты для каждого генома.

Название вида | Количество предсказанных Z-DNA | Количество участков с zh-score > 500 |	Общая длина участков
---|---|---|---
Phytomonas sp. isolate EM1 | | |
Phytomonas sp. isolate Hart1 | | |
Perkinsela sp. CCAP 1560/4 | | |
Leptomonas pyrrhocoris | | |
Leptomonas seymouri | | |

#### Гистограммы распределений

Название вида | Гистограмма
---|---
Phytomonas sp. isolate EM1 | ![image](https://user-images.githubusercontent.com/28685693/173230421-eb8468c7-b6af-48dc-bb3c-b6bd5066d3f8.png)
Phytomonas sp. isolate Hart1 | ![image](https://user-images.githubusercontent.com/28685693/173230429-1877a5fa-45ee-42a5-9c2a-1a95fd0ad9b9.png)
Perkinsela sp. CCAP 1560/4 | ![image](https://user-images.githubusercontent.com/28685693/173230437-14cfd261-4f10-46e5-b2f8-b44a52a4708e.png)
Leptomonas pyrrhocoris |![image](https://user-images.githubusercontent.com/28685693/173230452-1432c5e0-dd28-44d3-ad14-717757a96b85.png)
Leptomonas seymouri | ![image](https://user-images.githubusercontent.com/28685693/173230473-8dff0b3b-3180-436a-bb16-5565eb4192bf.png)

# Ассоциируем предсказанные участки Z-DNA с промотерами генов

#### Визуализация генов и предсказанных участков Z-DNA с помощью GraphicFeature, GraphicRecord

На картинках ниже изображено по одной Z-DNA на промотере гена для 5 генов из генома

Название вида | Визуализация
---|---
Phytomonas sp. isolate EM1 | ![image](https://user-images.githubusercontent.com/28685693/173230538-21d90cac-2ddd-4d71-ad03-51d3d8d9008d.png)
Phytomonas sp. isolate Hart1 | ![image](https://user-images.githubusercontent.com/28685693/173230541-cee2ad4e-98ca-456a-b111-580e7206fd7d.png)
Perkinsela sp. CCAP 1560/4 | ![image](https://user-images.githubusercontent.com/28685693/173230546-c3bfc7b1-7c66-48d7-b4a2-c73e668f6957.png)
Leptomonas pyrrhocoris | ![image](https://user-images.githubusercontent.com/28685693/173231404-afe129d2-0635-46f8-bce7-b9ec721dae81.png)
Leptomonas seymouri | ![image](https://user-images.githubusercontent.com/28685693/173231406-9af419c6-6d10-4008-a307-b2b085348c0b.png)


#### Визуализация генов и предсказанных участков Z-DNA с помощью IGV

Название вида | Визуализация
---|---
Phytomonas sp. isolate EM1 | 
Phytomonas sp. isolate Hart1 | 
Perkinsela sp. CCAP 1560/4 | 
Leptomonas pyrrhocoris | 
Leptomonas seymouri | 

#  Определяем гомологичные связи между белками выбранных геномов

#### Информация по полученным гомологичным кластерам
Общее число кластеров: 8114

Гистограмма кластеров по кол-ву разных геномов в кластере

![image](https://user-images.githubusercontent.com/28685693/173231479-75d0f12d-f942-46e3-8fa7-44bf71ea3c52.png)

#### Таблица с информацией по выбранным кластерам

Номер кластера | навзвание вида | product_accession | имя
0 | Phytomonas sp. isolate EM1 | CCW62705.1 | NaN
0 | Phytomonas sp. isolate Hart1 | CCW70538.1 | NaN
0 | Perkinsela sp. CCAP 1560/4 | KNH08991.1 | 26S proteasome non-ATPase regulatory subunit 7
0 | Leptomonas pyrrhocoris | KPA84532.1 | putative 26S proteasome regulatory subunit	
0 | Leptomonas seymouri | KPI89594.1 | putative Proteasome regulatory non-ATP-ase
1 | Phytomonas sp. isolate EM1 | CCW63896.1 | NaN
1 | Phytomonas sp. isolate Hart1 | CCW69870.1 | NaN
1 | Perkinsela sp. CCAP 1560/4 | KNH05598.1 | 19S proteasome regulatory subunit
1 | Leptomonas pyrrhocoris | KPA81485.1 | proteasome regulatory ATPase subunit (RPT6)	
1 | Leptomonas seymouri | KPI88447.1 | proteasome regulatory ATPase subunit (RPT6)
2 | Phytomonas sp. isolate EM1 | CCW65264.1 | NaN
2 | Phytomonas sp. isolate Hart1 | CCW66650.1 | NaN
2 | Perkinsela sp. CCAP 1560/4 | KNH09598.1 | hypothetical protein
2 | Leptomonas pyrrhocoris | KPA75841.1	| putative mitochondrial hypothetical protein
2 | Leptomonas seymouri | KPI86349.1 | hypothetical protein
3 | Phytomonas sp. isolate EM1 | CCW60596.1 | NaN
3 | Phytomonas sp. isolate Hart1 | CCW66587.1	| NaN
3 | Perkinsela sp. CCAP 1560/4 | KNH07404.1 | hypothetical protein
3 | Leptomonas pyrrhocoris | KPA82230.1	| putative Kinesin
3 | Leptomonas seymouri | KPI90442.1 | putative Kinesin
4 | Phytomonas sp. isolate EM1 | CCW65379.1	| NaN
4 | Phytomonas sp. isolate Hart1 | CCW72181.1	| NaN
4 | Perkinsela sp. CCAP 1560/4 | KNH07107.1 | cation-transporting ATPase
4 | Leptomonas pyrrhocoris | KPA74240.1 | putative mitochondrial cation-transporting ATPase
4 | Leptomonas seymouri | KPI83492.1 | putative cation-transporting ATPase
5 | Phytomonas sp. isolate EM1 | CCW64545.1	| NaN
5 | Phytomonas sp. isolate Hart1 | CCW72090.1	| NaN
5 | Perkinsela sp. CCAP 1560/4 | KNH08158.1	| hypothetical protein
5 | Leptomonas pyrrhocoris | KPA74355.1	| putative mitochondrial hypothetical protein
5 | Leptomonas seymouri | KPI88681.1 | hypothetical protein
6 | Phytomonas sp. isolate EM1 | CCW62673.1	| NaN
6 | Phytomonas sp. isolate Hart1 | CCW70506.1	| NaN
6 | Perkinsela sp. CCAP 1560/4 | KNH05304.1	| WD40 repeat-like protein
6 | Leptomonas pyrrhocoris | KPA84480.1	| putative Protein transport protein sec13
6 | Leptomonas seymouri | KPI89630.1 | putative Protein transport protein sec13
7 | Phytomonas sp. isolate EM1 | CCW64056.1 | NaN
7 | Phytomonas sp. isolate Hart1 | CCW69801.1	| NaN
7 | Perkinsela sp. CCAP 1560/4 | KNH09596.1	| hypothetical protein
7 | Leptomonas pyrrhocoris | KPA77180.1	| hypothetical protein
7 | Leptomonas seymouri | KPI84050.1 | hypothetical protein
8 | Phytomonas sp. isolate EM1 | CCW64935.1	| NaN
8 | Phytomonas sp. isolate Hart1 | CCW69598.1	| NaN
8 | Perkinsela sp. CCAP 1560/4 | KNH06676.1 | hypothetical protein
8 | Leptomonas pyrrhocoris | KPA78617.1	| putative mitochondrial mitochondrial carrier
8 | Leptomonas seymouri | KPI85475.1 | hypothetical protein
9 | Phytomonas sp. isolate EM1 | CCW61543.1	| NaN
9 | Phytomonas sp. isolate Hart1 | CCW68153.1	| NaN
9 | Perkinsela sp. CCAP 1560/4 | KNH08472.1	| tRNA (guanine-N(1)-)-methyltransferase
9 | Leptomonas pyrrhocoris | KPA83425.1	| hypothetical protein
9 | Leptomonas seymouri | KPI87030.1 | hypothetical protein

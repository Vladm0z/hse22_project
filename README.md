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

Так как работа проводилась с эукариотами, в таблице представлно число генов, длина генома, длина участков с экзонами и покрытие экзонами

Название вида | Число генов |	Длина генома | Длина участков с экзонами |	Доля покрытия экзонами
---|---|---|---|---
Phytomonas sp. isolate EM1 | 6381.0 | 17780869.0 | 9395487.0 | 52.8
Phytomonas sp. isolate Hart1 | 6451.0 | 18129152.0 | 8832047.0 | 48.7
Perkinsela sp. CCAP 1560/4 | 5252.0 | 9477801.0 | 5602200.0 | 59.1
Leptomonas pyrrhocoris | 10130.0 | 30379903.0 | 23471619.0 | 77.3
Leptomonas seymouri | 8597.0 | 27764161.0 | 15903750.0 | 57.3

---
# Предсказываем участки Z-DNA

Было произведено предсказание участков Z-DNA с помощью программы zhunt. После чего отобраны участки Z-DNA, имеющие zh-score больше 500.

Название вида | Количество предсказанных Z-DNA | Количество участков с zh-score > 500 
---|---|---
Phytomonas sp. isolate EM1 | 87160 | 7946
Phytomonas sp. isolate Hart1 | 91070 | 8392
Perkinsela sp. CCAP 1560/4 | 19196| 1742
Leptomonas pyrrhocoris | 393207 | 34665
Leptomonas seymouri | 31934 | 2816

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

#  Определяем гомологичные связи между белками выбранных геномов

#### Информация по полученным гомологичным кластерам
Общее число кластеров: 8114

Гистограмма кластеров по кол-ву разных геномов в кластере

![image](https://user-images.githubusercontent.com/28685693/173231479-75d0f12d-f942-46e3-8fa7-44bf71ea3c52.png)

#### Таблица с информацией по выбранным кластерам

Были рассмотрены кластеры, имеющие значения 5 в стобцах Species	и Genes

Номер кластера | навзвание вида | product_accession | имя
---|---|---|---
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

# Множественное белковое выравнивание

Для кластеров произведено множественное белоковое выравнивание на сайте https://www.ebi.ac.uk/Tools/msa/clustalo/. В качестве алгоритма для выравнивания был выбран алгоритм ```ClustalW with character counts```, результаты находятся в разделе data

# Визуализация расположения участков Z-DNA для каждого выбранного кластера

Номер кластера | Название вида | Визуализация
---|---|---
0 | Phytomonas sp. isolate EM1 | ![image](https://user-images.githubusercontent.com/28685693/173235512-a8409003-5de7-4eff-a94c-39a18c7059bd.png)
0 | Phytomonas sp. isolate Hart1 | ![image](https://user-images.githubusercontent.com/28685693/173235515-6fd4c8b4-7474-4674-b714-09212d8cead9.png)
0 | Perkinsela sp. CCAP 1560/4 | ![image](https://user-images.githubusercontent.com/28685693/173235518-ab18bda8-8384-4e30-a02f-15a7b7f428ab.png)
0 | Leptomonas pyrrhocoris | ![image](https://user-images.githubusercontent.com/28685693/173235521-406f2331-1a2d-4e7d-a37f-6a42b08d9954.png)
0 | Leptomonas seymouri | ![image](https://user-images.githubusercontent.com/28685693/173235522-a2ebd009-16cb-4b79-9ade-e7bfb8c18207.png)
1 | Phytomonas sp. isolate EM1 | ![image](https://user-images.githubusercontent.com/28685693/173234283-a303ead8-ef38-4206-9403-3fa4f245dc84.png)
1 | Phytomonas sp. isolate Hart1 | ![image](https://user-images.githubusercontent.com/28685693/173234285-b789604d-df66-4046-af30-13019e8fe7f3.png)
1 | Perkinsela sp. CCAP 1560/4 | ![image](https://user-images.githubusercontent.com/28685693/173234289-22801241-a461-4fd3-b769-e14f7cd1edc8.png)
1 | Leptomonas pyrrhocoris | ![image](https://user-images.githubusercontent.com/28685693/173234297-c093a344-624c-4792-8f01-caf58be2b85d.png)
1 | Leptomonas seymouri | ![image](https://user-images.githubusercontent.com/28685693/173234301-5d536761-886f-480e-acc0-5691a7a25243.png)
2 | Phytomonas sp. isolate EM1 | ![image](https://user-images.githubusercontent.com/28685693/173234305-fa3190ba-c71d-4ad1-b89d-64325514e9da.png)
2 | Phytomonas sp. isolate Hart1 | ![image](https://user-images.githubusercontent.com/28685693/173234312-2710193d-0e87-4f0e-92ab-484eabdfc468.png)
2 | Perkinsela sp. CCAP 1560/4 | ![image](https://user-images.githubusercontent.com/28685693/173234314-81a1d1ef-ffe1-4605-8a08-c3d3073418a3.png)
2 | Leptomonas pyrrhocoris | ![image](https://user-images.githubusercontent.com/28685693/173234317-71569fdb-3ba0-4906-81bc-68b2b1dc17c5.png)
2 | Leptomonas seymouri | ![image](https://user-images.githubusercontent.com/28685693/173234321-48bc39bf-3536-4cc2-a099-22350034bf54.png)
3 | Phytomonas sp. isolate EM1 | ![image](https://user-images.githubusercontent.com/28685693/173234324-2daf185f-ea45-4c7d-9914-6fa4fabb8aac.png)
3 | Phytomonas sp. isolate Hart1 | ![image](https://user-images.githubusercontent.com/28685693/173234327-a1944ddd-e926-46b1-9e5d-5a95ba746555.png)
3 | Perkinsela sp. CCAP 1560/4 | ![image](https://user-images.githubusercontent.com/28685693/173234333-5f85b0be-82e9-48a8-9137-18912a3fb787.png)
3 | Leptomonas pyrrhocoris | ![image](https://user-images.githubusercontent.com/28685693/173234336-d81741c7-238a-4ab2-b2fb-fb12b4555a3d.png)
3 | Leptomonas seymouri | ![image](https://user-images.githubusercontent.com/28685693/173234339-221dc54e-9e45-409e-b764-d988d735b0dc.png)
4 | Phytomonas sp. isolate EM1 | ![image](https://user-images.githubusercontent.com/28685693/173234344-85ed18d9-c089-481f-8515-c85f6dd9646e.png)
4 | Phytomonas sp. isolate Hart1 | ![image](https://user-images.githubusercontent.com/28685693/173234346-f1acc7de-a60f-4f6b-98e4-df1ce5158a3d.png)
4 | Perkinsela sp. CCAP 1560/4 | ![image](https://user-images.githubusercontent.com/28685693/173234354-24966a49-3ccd-4336-8c9c-58edb9885591.png)
4 | Leptomonas pyrrhocoris | ![image](https://user-images.githubusercontent.com/28685693/173234358-4c571b4f-941e-454f-b791-a4a20fbb1390.png)
4 | Leptomonas seymouri | ![image](https://user-images.githubusercontent.com/28685693/173234361-54c3dfa3-6ec9-4ef2-8486-1373e5810bc1.png)
5 | Phytomonas sp. isolate EM1 | ![image](https://user-images.githubusercontent.com/28685693/173235625-1c19eeb5-4564-49c0-9857-01896892e2a8.png)
5 | Phytomonas sp. isolate Hart1 | 
5 | Perkinsela sp. CCAP 1560/4 | 
5 | Leptomonas pyrrhocoris | 
5 | Leptomonas seymouri | 
6 | Phytomonas sp. isolate EM1 | ![image](https://user-images.githubusercontent.com/28685693/173234379-58961603-2057-4184-886c-40e5219e56c2.png)
6 | Phytomonas sp. isolate Hart1 | ![image](https://user-images.githubusercontent.com/28685693/173234380-45ad9268-ce68-46f6-9978-d7882d6467eb.png)
6 | Perkinsela sp. CCAP 1560/4 | ![image](https://user-images.githubusercontent.com/28685693/173234383-48b030df-a9ce-452d-b8c4-4ffda98360b8.png)
6 | Leptomonas pyrrhocoris | ![image](https://user-images.githubusercontent.com/28685693/173234385-85f917e0-c2fc-48f5-b1c7-111743da2aed.png)
6 | Leptomonas seymouri | ![image](https://user-images.githubusercontent.com/28685693/173234390-88cffa7a-2b78-4fa6-9ea4-483fa7bbb8e6.png)
7 | Phytomonas sp. isolate EM1 | ![image](https://user-images.githubusercontent.com/28685693/173235531-6ccb6ded-243a-4f62-a468-2ff9a5ce5d92.png)
7 | Phytomonas sp. isolate Hart1 | ![image](https://user-images.githubusercontent.com/28685693/173235533-40990e08-481c-41b1-a06f-dc17bd699cea.png)
7 | Perkinsela sp. CCAP 1560/4 | ![image](https://user-images.githubusercontent.com/28685693/173235538-d4a103d5-db45-4054-9d4e-960a59906dbe.png)
7 | Leptomonas pyrrhocoris | ![image](https://user-images.githubusercontent.com/28685693/173235543-a9c0843f-565b-49e0-bf2f-6bdf2850154c.png)
7 | Leptomonas seymouri | ![image](https://user-images.githubusercontent.com/28685693/173235545-48b340c0-9d5d-42c0-a570-63d99640970f.png)
8 | Phytomonas sp. isolate EM1 | ![image](https://user-images.githubusercontent.com/28685693/173235615-e0fe8e4f-1620-46c4-932d-1765649bed0a.png)
8 | Phytomonas sp. isolate Hart1 | ![image](https://user-images.githubusercontent.com/28685693/173235617-5043dd2b-7a70-4dfc-ba35-6d868e02fba4.png)
8 | Perkinsela sp. CCAP 1560/4 | 
8 | Leptomonas pyrrhocoris | 
8 | Leptomonas seymouri | 
9 | Phytomonas sp. isolate EM1 | ![image](https://user-images.githubusercontent.com/28685693/173235589-cbaebdee-435f-4a7f-a4d5-b46cfca88284.png)
9 | Phytomonas sp. isolate Hart1 | ![image](https://user-images.githubusercontent.com/28685693/173235592-857fda32-2aa7-4042-8496-b94fa01a6f35.png)
9 | Perkinsela sp. CCAP 1560/4 | ![image](https://user-images.githubusercontent.com/28685693/173235598-6f039310-08df-43dc-b332-8d467f893ecb.png)
9 | Leptomonas pyrrhocoris | ![image](https://user-images.githubusercontent.com/28685693/173235601-1bfa4d01-6bdb-4b3e-9a58-2f71e391098d.png)
9 | Leptomonas seymouri | ![image](https://user-images.githubusercontent.com/28685693/173235603-648e2867-f963-4ccc-9ce8-32778a3386a5.png)

# hse_hw3_chromhmm
## Ссылка на колаб: https://colab.research.google.com/drive/193snh9H5_MF-8TT60o5FTJj77RMgB8DC?usp=sharing
# Исходные данные
Клеточная линия: HUVEC (тк MM.1S из ДЗ2 нет в таблице)
## Table1
Клеточная линия | Гистоновая метка | Имя файла | Файл с контролем 
| --- | --- | --- | ---
HUVEC|H3k27me3|H3k27me3StdAlnRep1.bam|ControlStdAlnRep1.bam
HUVEC|H3k4me1|H3k4me1StdAlnRep1.bam|ControlStdAlnRep1.bam
HUVEC|H3k4me2|H3k4me2StdAlnRep1.bam|ControlStdAlnRep1.bam
HUVEC|H3k4me3|H3k4me3StdAlnRep1.bam|ControlStdAlnRep1.bam
HUVEC|H3k9me1|H3k9me1StdAlnRep1.bam|ControlStdAlnRep1.bam
HUVEC|H4k20me1|H4k20me1StdAlnRep1.bam|ControlStdAlnRep1.bam
HUVEC|Pol2b|Pol2bStdAlnRep1.bam|ControlStdAlnRep1.bam
HUVEC|H3k27ac|H3k27acStdAlnRep1.bam|ControlStdAlnRep1.bam
HUVEC|Ctcf|CtcfStdAlnRep1.bam|ControlStdAlnRep1.bam
HUVEC|H3k36me3|	H3k36me3StdAlnRep1.bam|ControlStdAlnRep1.bam

# Выдача после ChromHMM
| ![image](https://user-images.githubusercontent.com/93148620/160017097-04d93d04-7873-40d9-b1b6-0b9fc3ac3301.png) | ![image](https://user-images.githubusercontent.com/93148620/160017308-68667b50-f7f4-4d21-85cc-f0009d7d47c4.png) | ![image](https://user-images.githubusercontent.com/93148620/160017376-274679ca-ff56-4c60-bbb8-822862f6bde3.png) | ![image](https://user-images.githubusercontent.com/93148620/160017453-e31c5886-85a4-4558-8cf7-7ce1a5d97693.png) | ![image](https://user-images.githubusercontent.com/93148620/160017516-88e7813b-8743-47ae-8c86-298f46a83e2f.png) |
| ------------- | ------------- |--------------------| -- | -- |

## Table2
|Состояние|1|2|3|4|5|6|7|8|9|10|
|--|--|--|--|--|--|--|--|--|--|--|
|Метки|H3k4me3,H3k4me2,немного H3k4me1|H3k4me3,H3k4me2,H3k27ac,немного H3k4me1 и Pol2b |H3k4me2,H3k27ac,H3k4me1|H3k4me1|H3k4me1,H3k36me3,немного Pol2b|H3k36me3|немного Pol2b|немного Pol2b|H3k27me3|Ctcf|
|Часть генома|CpG island, экзоны, гены,старт транскрипции|CpG island, экзоны, гены,старт транскрипции|гены,ядерная ламина,конец транскрипции|гены, конец транскрипции,ядерная ламина|экзоны, гены, конец транскрипции|экзоны, гены, конец транскрипции|гены,конец транскрипции,ядерная ламина|много в геноме, ядерная ламина|ядерная ламина|ядерная ламина, конец транскрипции, экзоны|
|Расположение относительно TSS(старт транскрипции)|на TSS(максимум находится на старте и далее спад в обе стороны)|на TSS(максимум находится на старте и далее спад в обе стороны)|-|-|после TSS немного|-|немного до и после TSS|-|постоянное расположение на всём промежутке|немного на TSS и далее спад в обе стороны|
|Расположение относительно TES(конец транскрипции)|до, на, после TES|до, на, после TES|немного до, на и после|немного до, на и после TES|до, на и после (на TES больше всего)|до, на, после TES(до больше всего)|до, на и после TES|-|немного до, на и после|до, на и после(после больше всего)|
|Итог|Active promoter|Active promoter|Strong Enhancer|Enhancer|Enhancer|Transcribed region|Heterochromatin|Heterochromatin|Polycomb-repressed|Weak promoter|

# Биологическая роль гистоновых меток
## Table3
|Метка|Имя файла|Роль|
|:--|--|--:|
|H3k27me3|H3k27me3StdAlnRep1.bam|Формирование гетерохроматических областей и понижением регуляции близлежащих генов (downregulation)|
|H3k4me1|H3k4me1StdAlnRep1.bam|Ассоциируется с энхансерами (gene enhancers)|
|H3k4me2|H3k4me2StdAlnRep1.bam|Ассоциирована с активацией генов|
|H3k4me3|H3k4me3StdAlnRep1.bam|Связана с активацией транскрипции близлежащих генов, связана с промоторами|
|H3k9me1|H3k9me1StdAlnRep1.bam|Связана с местом начала транскрипции активных генов|
|H4k20me1|H4k20me1StdAlnRep1.bam|Связана с активацией транскрипции|
|Pol2b|Pol2bStdAlnRep1.bam|Кодируют ДНК-полимеразу,которая обеспечивает точную репликацию генома|
|H3k27ac|H3k27acStdAlnRep1.bam|Связан с более высокой активацией транскрипции и поэтому определяется как активный энхансер.|
|Ctcf|CtcfStdAlnRep1.bam|Транскрипционная регуляция и регуляция структуры хроматина (транскрипционный фактор)|
|H3k36me3|H3k36me3StdAlnRep1.bam|Связана с телами генов,также может быть вовлечена в определение экзонов.|

# Данные из геномного браузера
| ![image](https://user-images.githubusercontent.com/93148620/160277183-2272cead-866d-48f5-b127-c78d5161a7dc.png) | ![image](https://user-images.githubusercontent.com/93148620/160277198-67e3ce60-5c6a-4372-9a78-390900fb460a.png) | ![image](https://user-images.githubusercontent.com/93148620/160277227-825b5baf-bfdb-4e52-aed6-a4147420dba1.png) | ![image](https://user-images.githubusercontent.com/93148620/160277250-6082c308-af98-44af-b8b8-6ab528ebc221.png) | ![image](https://user-images.githubusercontent.com/93148620/160277326-a9824ff3-8833-451d-8661-40ce1c3fb1a2.png) |
| ------------- | ------------- |--------------------| -- | -- |


 
# Команды
 ### Binarize Bam
```python
!java -mx5000M -jar /content/ChromHMM/ChromHMM.jar BinarizeBam -b 200  /content/ChromHMM/CHROMSIZES/hg19.txt /content/ cellmarkfiletable.txt   binarizedData
```
### Learn Module
```python
!java -mx5000M -jar /content/ChromHMM/ChromHMM.jar LearnModel -b 200 /content/binarizedData/ /content/learnmodel/ 10 hg19
!zip -r learmodel.zip learnmodel/
```
# Бонусное задание

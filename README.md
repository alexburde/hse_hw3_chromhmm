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
|Метки|||||||||||
|Часть генома|||||||||||
|Расположение относительно TSS|||||||||||
|Расположение относительно TES|||||||||||
|Итог|||||||||||

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

Картинка | Состояние 
| --- | --- 
<img width="629" alt="image" src="https://user-images.githubusercontent.com/93148620/160138272-f1984eb1-5f12-4746-89b0-389ac0e48cce.png">|1
<img width="622" alt="image" src="https://user-images.githubusercontent.com/93148620/160138797-38b3392b-8316-49a9-92a2-6f11aa081028.png">|2
<img width="469" alt="image" src="https://user-images.githubusercontent.com/93148620/160140640-1b6165eb-51be-4174-9526-223eda680044.png">|3
<img width="623" alt="image" src="https://user-images.githubusercontent.com/93148620/160141409-918a6f83-1007-467c-9af4-5ef92805062f.png">|4
<img width="465" alt="image" src="https://user-images.githubusercontent.com/93148620/160142329-edfe1553-2026-412e-a2ce-e635033d745f.png">|5
<img width="626" alt="image" src="https://user-images.githubusercontent.com/93148620/160140035-838e4478-7a36-4e79-b66a-49ffed695477.png">|6
<img width="469" alt="image" src="https://user-images.githubusercontent.com/93148620/160139756-2a3b0b8c-5cf1-4d08-85dd-1a9fd0f1c65b.png">|7
<img width="628" alt="image" src="https://user-images.githubusercontent.com/93148620/160137474-aa9119c2-be6b-460c-aa23-330b06ea9624.png">|8
<img width="469" alt="image" src="https://user-images.githubusercontent.com/93148620/160142194-c635919a-3093-4ed4-840e-291ca3906552.png">|9
<img width="628" alt="image" src="https://user-images.githubusercontent.com/93148620/160141741-1112f1fd-e76b-4aa5-a5c1-3ce10cd5c9ae.png">|10
 
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

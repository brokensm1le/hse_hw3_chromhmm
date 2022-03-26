# hse_hw3_chromhmm

Задание было выполнено для клеточной линии: `Huvec`.

Ссылка на *GoogleColab*: https://colab.research.google.com/drive/1mhrtzEmvPfNIupvTPz2-6cDMCSon27ht?usp=sharing

## Часть 1

#### Таблица с используемыми гистоновыми метками:

| Название гистоновой метки | Имя файла |
| ------- | ----------- |
| H2az	| H2azAlnRep1.bam	|
| H3k27ac |	H3k27acStdAlnRep1.bam	|
|	H3k27me3 |	H3k27me3StdAlnRep1.bam  |
|	H3k36me3 |	H3k36me3StdAlnRep1.bam  |
|	H3k4me1 |	H3k4me1StdAlnRep1.bam	|
|	H3k4me2 |	H3k4me2StdAlnRep1.bam	|
|	H3k4me3 |	H3k4me3StdAlnRep1.bam	|
|	H3k79me2 |	H3k79me2AlnRep1.bam	|
| H3k9ac |	H3k9acStdAlnRep1.bam	|
| H3k9me1 |	H3k9me1StdAlnRep1.bam	|

#### Полученные изображения после ChromHMM:

<p float="left">
  <img src="/ChromHMM_output/emissions_10.png" width="330" />
  <img src="/ChromHMM_output/transitions_10.png" width="330" />
  <img src="/ChromHMM_output/Huvec_10_overlap.png" width="330" />
  <img src="/ChromHMM_output/Huvec_10_RefSeqTSS_neighborhood.png" width="400" />
  <img src="/ChromHMM_output/Huvec_10_RefSeqTES_neighborhood.png" width="400" />
</p>

#### Таблица c обозначениями эпигенетических типов:

| State | Описание                                    | Название эпигенетического типа |
| ----- | ------------------------------------------- | ------------------------------ |
|   1   | Гистоновые Mодификации:NA. Показывает низкий сигнал.| Repressed |
|   2   | ГМ:`H2azAlnRep1.bam` и `H3k27me3StdAlnRep1.bam`. Чаще всего ассоциировано с ядерной ламиной. Показывает средний сигнал. | Heterochromatin |
|   3   |	ГМ:`H2azAlnRep1.bam` и `H3k27me3StdAlnRep1.bam`. Показывает средний сигнал.| Repressed |
|   4   |	ГМ:`H2azAlnRep1.bam`. Показывает низкий сигнал. Большой процент в CpG откровков.| Enhancer |
|   5   |	ГМ:`H3k4me2(3)StdAlnRep1.bam`, `H3k27acStdAlnRep1.bam`,`H3k79me2AlnRep1.bam`. Показывает высокий сигнал. Большой процент в CpG откровков. Большой процент Exon. | Promoter |
|   6   |	ГМ:`H3k4me1StdAlnRep1.bam`, `H3k27acStdAlnRep1.bam`. Показывает высокий сигнал. | Enhancer |
|   7   |	ГМ:NA. Показывает низкий сигнал.    | Transcribed |
|   8   |	ГМ:`H3k4me2StdAlnRep1.bam` и `H3k79me2AlnRep1.bam`. Показывает высокий сигнал. | Promoter |
|   9   | ГМ:`H3k79me2AlnRep1.bam`. Показывает средний сигнал.  | Enhancer |
|   10  | ГМ:NA. Показывает низкий сигнал.	  | Transcribed |


#### Таблица с примерами/скринами:

| State | Скрин с genome.ucsc                      |
| ----- | ---------------------------------------- |
|   1   | <img src="/pic/1_bio.png" width="200" /> |
|   2   | <img src="/pic/2_bio.png" width="200" /> |
|   3   |	<img src="/pic/3_bio.png" width="200" /> |
|   4   |	<img src="/pic/4_bio.png" width="200" /> |
|   5   |	<img src="/pic/5_bio.png" width="200" /> | 
|   6   |	<img src="/pic/6_bio.png" width="200" /> |
|   7   |	<img src="/pic/7_bio.png" width="200" /> |
|   8   |	<img src="/pic/8_bio.png" width="200" /> |
|   9   | <img src="/pic/9_bio.png" width="200" /> |
|   10  | <img src="/pic/10_bio.png" width="200" />|

## Part 2 (BONUS)
<img src="/pic/bonus.png" width="800" />

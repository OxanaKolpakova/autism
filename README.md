# autism
Comparative analysis of patients with autism and healthy people based on NGS data

Описание задачи:
ИЦиГ, Новосибирск, WES/аутизм, Трифонова ЕА, к.б.н.
Подтверждение удовлетворительного качества секвенирования на GenolabM, GeneMind под определенную задачу, WES/аутизм
Сесана предоставит: 2FCH PE 150, оплата статьи; набор WES Raissol
в печать:12.2024, ТрифоноваЕА, Колпакова ОА, Глебус АС

Расстройства аутистического спектра (РАС) относятся к комплексным нарушениям нейропсихического развития, процент диагностирования которых постоянно растет последние полвека.

Так, в 1995 году диагностировался с РАС 1 ребенок из 500, а через 20 лет (в 2015 году) уже 1 из 68 детей по данным Центра по контролю и профилактике заболеваний США (www.cdc.gov/ncbddd/autism/data. html). 

Аутизм относится к крайне высоко наследуемым заболеваниям с очень сложной генетикой, к настоящему времени выявлено более 1000 генов предрасположенности.

Нами подобраны 2 когорты пациентов: 1. молодые люди с аутизмом в возрасте 25+ лет и 2. дети с аутизмом в возрасте 4-7 лет. В ходе исследований мы предполагаем сравнить полноэкзомные сиквенсы для этих когорт и попытаться выяснить, вносит ли генетический фактор (увеличение количества SNP, делеций и дупликаций) существенный вклад в повышение уровня диагностирования аутизма.

Расстройства аутистического спектра (РАС) относятся к комплексным нарушениям нейропсихического развития, процент диагностирования которых постоянно растет последние полвека. 
Так, в 1995 году диагностировался с РАС 1 ребенок из 500, а через 20 лет (в 2015 году) уже 1 из 68 детей по данным Центра по контролю и профилактике заболеваний США (www.cdc.gov/ncbddd/autism/data. html). 

Аутизм относится к крайне высоко наследуемым заболеваниям с очень сложной генетикой, к настоящему времени выявлено более 1000 генов предрасположенности.	
https://docs.google.com/spreadsheets/d/1hEm6luKk1akN3jj2OYLnpw2y58iBxlLiwUmYkK7o-_s/edit?gid=0#gid=0	

Литература:
WES_autism        https://www.ncbi.nlm.nih.gov/myncbi/collections/64219611/
met_autism        https://www.ncbi.nlm.nih.gov/myncbi/collections/64219733/

GeneMind:

1: Li C, Fan X, Guo X, Liu Y, Wang M, Zhao XC, Wu P, Yan Q, Sun L. 
Accuracy benchmark of the GeneMind GenoLab M sequencing platform for WGS and WES analysis. BMC Genomics. 2022 Jul 22;23(1):533. doi: 10.1186/s12864-022-08775-3. PMID: 35869426; PMCID: PMC9308344.

https://pubmed.ncbi.nlm.nih.gov/36882687/

2: Pavel I, Irina L, Tatiana G, Denis P, Philipp K, Sergei K, Evgeny D.
Comparison of the Illumina NextSeq 2000 and GeneMind Genolab M sequencing platforms for spatial transcriptomics. BMC Genomics. 2023 Mar 7;24(1):102. doi: 10.1186/s12864-023-09192-w. PMID: 36882687; PMCID: PMC9990361.

https://pubmed.ncbi.nlm.nih.gov/38707210/

3: Ru B, Wang T, Liu Y, Zhao X, Lei M. 
The complete chloroplast genome sequence of leibnitzia anandria (linnaeus) turczaninow. Mitochondrial DNA B Resour. 2024 May 2;9(5):578-582. doi: 10.1080/23802359.2024.2347511. PMID: 38707210; PMCID: PMC11067557.

https://pubmed.ncbi.nlm.nih.gov/36721080/

4: Feng B, Lai J, Fan X, Liu Y, Wang M, Wu P, Zhou Z, Yan Q, Sun L. 
Systematic comparison of variant calling pipelines of target genome sequencing cross multiple next-generation sequencers. Front Genet. 2024 Jan 4;14:1293974. doi: 10.3389/fgene.2023.1293974. PMID: 38239851; PMCID: PMC10794554.

MGI: https://pubmed.ncbi.nlm.nih.gov/32176719/



Планирование эксперимента, анализ

## Какой анализ мы проводим?

1. Сравнение больных и здоровых. Решить можем ли мы взять здоровых только с MGI? Можем, если нет отличия между выботками по различны секвенаторам (concordance rate по контрольной библиотеке).
    Смущает другая технология. Или взять данные Illumina, Томский НИМЦ

- Хи-квадрат. Сравниваем каждую позицию: миллионы тестов -> Порправка на множественное сравнение -> Мощность? 
- Проблема множественного сравнения. Решение: https://www-ncbi-nlm-nih-gov.translate.goog/pmc/articles/PMC5003626/?_x_tr_sl=ja&_x_tr_tl=ru&_x_tr_hl=ru&_x_tr_pto=wapp
- Проблема рассчета мощности
- Мы берем все гены или только 1000. (Если 1000 тогда какой научный интерес)
- Мы ищем различия или доказываем идентичность? (Если  идентичность, надо искать методику теста)

2.  Сравнение детей и взрослых. Определиться с 0 гипотезой, что мы хотим проверить.

- Мощность?

3.  Сравнение MGI и генолаба? подумать про корректность, другой принцип. Можем взять контроль Iliumina, попросить Томский НИМЦ данные контрольных библиотек, здоровых
- Можно добавить людей из иллюмины, это повысит мощность. 
- Нужно провоодить дополнительное исследование. Доказывать репрезентативность
- Есть риск получить отличия

4.  Поиск подтипов болезни
- Кластеризация
- Нужно больше людей для мощности
- Проблема субпопуляция, надо кластеризировать каждую субпопуляцию

5. поиск перепредставленных путей по GO? https://wiki.uio.no/projects/clsi/images/0/0a/GeneOntologyAndORA-2015.pdf



Пример структуры данных
Если у вас есть данные по двум группам и каждому варианту, таблица может выглядеть так:

## 1.1 Пример сводной таблицы для Хи-квадрат

| Variant ID | Group   | Present | Absent | Total |
|------------|---------|---------|--------|-------|
| rs123456   | Sick    | 40      | 60     | 100   |
| rs123456   | Healthy | 10      | 90     | 100   |
| rs789101   | Sick    | 30      | 70     | 100   |
| rs789101   | Healthy | 15      | 85     | 100   |
...
Примерно 10000 - 100000 на экзом.

## 1.2 Рассчет объема выборки для хи квадрат

```R
library(pwr)
# Задаем параметры
effect_size <- 0.3  # Средний эффект
alpha <- 0.05  # Уровень значимости
power <- 0.8  # Мощность теста
df <- 2   # Степени свободы для 3x2 таблицы
# Расчет объема выборки
sample_size <- pwr.chisq.test(w = effect_size, df = df, sig.level = alpha, power = power)
sample_size
```

Chi squared power calculation
w = 0.3
N = 107.0521
df = 2
sig.level = 0.05
power = 0.8
NOTE: N is the number of observations

107 человек для среднего эффекта без учета поправок

```R
library(pwr)
# Задаем параметры
effect_size <- 0.3  # Средний эффект https://www.utstat.toronto.edu/~brunner/oldclass/378f16/readings/CohenPower.pdf (p. 227, p.249)
alpha <- 0.05 / 10000  # Скоррекрированный уровень значимости
power <- 0.8  # Мощность теста
df <- 2   # Степени свободы для 3x2 таблицы
# Расчет объема выборки
sample_size <- pwr.chisq.test(w = effect_size, df = df, sig.level = alpha, power = power)
sample_size
```



Chi squared power calculation
w = 0.3
N = 359.4392
df = 2
sig.level = 5e-06
power = 0.8
NOTE: N is the number of observations

360 человек для среднего эффекта с учетом поправки Бонферони

## 2 Сравнение детей и взрослых

## 3 Сравнение иллюмины и генолаба
- Провести анализ конкордантности. Нужны ли контрольные библиотеки?
concordance rate
- или просто GC. Этого достаточно?

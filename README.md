# ChIP-Seq    
Работа сделана для клеточной линии A549 и гистоновой метки H3K9me3  
    
[Работа в Google Colab](https://colab.research.google.com/drive/1Qx5wpjsFQng5nsC2iQZvXUyzIVSnmVcf?usp=sharing)

## FastQC
    
### Реплика 1 ENCFF860ZHN
![image](data/ZHN_1.png)
![image](data/ZHN_2.png)
![image](data/ZHN_3.png)
![image](data/ZHN_4.png)
![image](data/ZHN_5.png)
![image](data/ZHN_6.png)
### Реплика 2 ENCFF410QJG
![image](data/QJG_1.png)
![image](data/QJG_2.png)
![image](data/QJG_3.png)
![image](data/QJG_4.png)
![image](data/QJG_5.png)
![image](data/QJG_6.png)
### Контроль ENCFF524OKJ
![image](data/OKJ_1.png)
![image](data/OKJ_2.png)
![image](data/OKJ_3.png)
![image](data/OKJ_4.png)
![image](data/OKJ_5.png)
![image](data/OKJ_6.png)    
    
Подрезание чтений не потребовалось, так как качестов было хорошее.
## Выравнивание чтений по 13 хромосоме    
Таблица выравнивания чтений:    
File | Общее число ридов | Выровнившиеся уникально | (%) | Выровнившиеся неуникально | (%) | Не выровнившиеся | (%)
--- | --- | --- | --- | --- | --- | --- | ---
ENCFF860ZHN | 49709602 | 2090897 | 4.21% | 7541175 | 15.17% | 40077530 | 80.62%
ENCFF410QJG | 25569991 | 1116143 | 4.37% | 4314823 | 16.87% | 20139025 | 78.76%
ENCFF524OKJ | 27267571 | 971508 | 3.56% | 2927915 | 10.74% | 23368148| 85.70%

Процент выравнивания невысовкий, потому что выравнивание производилось только по одной хромосоме.

## Пересечение MACS2 пиков и ENCODE пиков
Диаграммы Венна:     
ENCFF860ZHN и ENCODE
![image](data/venn1.png)    
ENCODE и ENCFF860ZHN
![image](data/venn2.png)    
ENCFF410QJG и ENCODE
![image](data/venn3.png)     
ENCODE и ENCFF410QJG
![image](data/venn4.png)    
    
Пересечений пиков очень мало, из-за того что выранивание производилось на одну хромомсому, также при подсчёте пересечений MACS2 пиков с ENCODE и наоборот может быть разное количество пересечений, но из-за очень малого количества пересечений это не было отображено.

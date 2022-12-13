# IHW3_bioinformatics
Индивидуальное задание 3 по биоинформатике
## Бесшапов Алексей, группа 2
### Геномы SARS-CoV-2 взяты из стран:
- США
- Индия
- Египет
- Филиппины
- Китай
- Германия
- Италия
- Великобритания
- Россия
### Процесс работы
Для начала, требуется провести выравнивание последовательностей с использованием алгоритма Muscle. Получим выравнивание:
<img width="958" alt="SARS-CoV-genomes" src="https://user-images.githubusercontent.com/45789410/207372727-96f708be-43c2-49f5-89ca-a5bb8ad2d9b0.png">

Далее построим деревья методом расстояний, методом максимальной бережливости и методом максимального правдоподобия.

Метод расстояний:

<img width="684" alt="SARS-CoV-genomes_NJ" src="https://user-images.githubusercontent.com/45789410/207374263-8bfe73c6-d906-467f-b805-ab5f07600eae.png">

Метод максимальной бережливости:

<img width="684" alt="SARS-CoV-genomes_MP" src="https://user-images.githubusercontent.com/45789410/207374382-4575f30f-3ef2-479a-8916-d72a9d2b55f5.png">

Метод максимального правдоподобия:

<img width="740" alt="SARS-CoV-genomes_ML" src="https://user-images.githubusercontent.com/45789410/207374458-4c0072c2-1f0e-4ff9-afd6-a1c732a7775d.png">

Судя по деревьям, построенным с помощью методов расстояний и максимального правдоподобия, самым первым был заражен итальянец, а последним - американец.

Судя по дереву, построенному с помощью метода максимальной бережливости, самым первым был заражен филиппинец, а последним - американец.

Рассмотрим отдельно пары Италия - Америка и Филиппины - Америка.

#### Италия - Америка: строим выравнивание:

<img width="956" alt="SARS-CoV-genomes-separate-USA-ITA" src="https://user-images.githubusercontent.com/45789410/207376154-9430b90d-9766-42ec-81b9-02d82dcbc322.png">

Возьмем пять мутаций: 

координаты 1-17:

<img width="532" alt="mutation1-17-USA-ITA" src="https://user-images.githubusercontent.com/45789410/207376563-3121587a-9006-4ed7-9fd6-59d652be60ec.png">

координаты 486-494:

<img width="462" alt="mutation486-494-USA-ITA" src="https://user-images.githubusercontent.com/45789410/207376696-d7503cab-7a04-4f55-bfa6-c218eee1ae07.png">

координата 646:

<img width="394" alt="mutation646-USA-ITA" src="https://user-images.githubusercontent.com/45789410/207377402-5259921b-f86c-4b6b-aea3-319293f2118b.png">

координата 1907:

<img width="394" alt="mutation1907-USA-ITA" src="https://user-images.githubusercontent.com/45789410/207377470-da60b50a-5769-45c9-b6a7-6dd9b343b1af.png">

координата 2120:

<img width="393" alt="mutation2120-USA-ITA" src="https://user-images.githubusercontent.com/45789410/207377533-159aacd3-5de9-413d-ad02-a9cbf1506704.png">

##### Итого: первая мутация произошла в некодирующем участке в начале генома, перед геном ORF1ab. Остальные - в гене ORF1ab.

#### Филиппины - Америка: строим выравнивание:

<img width="959" alt="SARS-CoV-genomes-separate-USA-PHL" src="https://user-images.githubusercontent.com/45789410/207380931-b946a95e-b196-464a-9480-2718953f5b56.png">


*Если не открывает файл, то перейти по [ссылке](https://nbviewer.jupyter.org/github/kotl68/Yandex_learning_project/blob/master/%D0%9F%D1%80%D0%BE%D0%B3%D0%BD%D0%BE%D0%B7%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5%20%D0%B2%D0%B5%D1%80%D0%BE%D1%8F%D1%82%D0%BD%D0%BE%D1%81%D1%82%D0%B8%20%D0%BE%D1%82%D1%82%D0%BE%D0%BA%D0%B0%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D0%B5%D0%B9%20%D0%B4%D0%BB%D1%8F%20%D1%84%D0%B8%D1%82%D0%BD%D0%B5%D1%81-%D1%86%D0%B5%D0%BD%D1%82%D1%80%D0%BE%D0%B2/prediction.ipynb)*

# Прогнозирование вероятности оттока пользователей для фитнес-центров
## Задача проекта  
На основе данных о посетителях сети фитнес-центров спрогнозировать вероятность оттока для каждого клиента в следующем месяце, сформировать с помощью кластеризации портреты пользователей
## Описание проекта 
В данном проекте использовано машинное обучение. Спрогнозирована вероятность
оттока (на уровне следующего месяца) для каждого клиента; сформированы типичные
портреты пользователей: выделены наиболее яркие группы, охарактеризованы их
основные свойства; проанализированы основные признаки, наиболее сильно влияющие
на отток.
## Выводы
####  Качество данных
Хорошо бы иметь больше данных для построения более качественной модели клиента. Т.к не известно за какой период собраны эти данные, может они уже не актуальны. В какой валюте тратят клиенты деньги, на что именно. По этим параметрам можно составить и доработать модель клиента. Какие групповые занятия посещают и т.к

#### Общие характеристики клиентов, которые склонны к оттоку
Самые важные причины, влияющие на отток пользователей, следующие:

- меньший возраст
- отсутствие проживания или работы в районе, где находится фитнес-центр
- маленькая продолжительность контракта,
- низкий уровень партнерских программ и акции "приведи друга" 
-  низкий факт посещения групповых занятий

#### Рекомендации
Для группы пользователей кластера `0` и `4` лучше ничего не делать, пока показатели не изменяться. Зачем влезать туда что и так хорошо работает

`1` кластеру можно предложить новые групповые занятия или скидку,бесплатную услугу от фитнес-центра: кафе, спорт-товары, косметический и массажный салон т.к их показатели высоки и им чего-то не хватает. Здесь надо провести более детальный анализ.
Но этим людям не надо быть навязчивыми это может их отпугнуть т.к они не оставляли свой номер телефона. Это может говорить о том что лишний спам им не нужен.

`2` кластер. Это люди которые не проживанию или работают в районе, где находится фитнес-центр. Так же у них низкий показатель акции «приведи друга» и факт посещения групповых занятий. Возможно, им скучно заниматься одним или они находят фитнес-центр поближе к дому или работе. Можно попробовать предложить им побольше групповых занятий, там они могут познакомиться с людьми и вместе ходить в зал и тогда расстояние покажется незначительной проблемой.

`3` кластер. Это самая большая группа людей и так же они самая молодая группа. Они посещают реже всех фитнес-центр, может дело в работе, нехватает мотивации или дело в сезоне. Ведь неизвестно когда они уходили. Им можно предложить скидку на абонемент для дополнительной мотивации или сделать упор на другие услуги фитнес-центра, вроде массажа, сауны, бассейна чтобы они могли расслабиться после работы. 

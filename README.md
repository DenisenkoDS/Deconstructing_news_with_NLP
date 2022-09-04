# Деконструкция новостей
# Topic modeling - Named-entity recognition - Exploratory data analysis
## Elbrus bootcamp - 2022 - Final project

### Деконструкция новостей - это пакет инструментов для динамичного и адаптивного анализа большого корпуса постов ТГ каналов. 

Датасет, с которым мы работали, включает в себя тексты из 6 популярных новостных ТГ каналов с 1 июля 2021 по 1 июля 2022 года. Всего у нас больше 110 тысяч текстов. В этот датасет можно быстро и просто добавлять новые блоки данных.

Мы использовали модель латентного размещения Дирихле (Latent Dirichlet allocation, LDA) от SciKitLearn для тематического моделирования. LDA позволяет автоматически разделить текст на стабильные кластеры и выделить ключевые слова в каждом кластере.

Дальше мы решаем задачу распознавания именнованных сущностей. Имена людей, названия организаций и другие имена собственные - это именнованные сущности. Мы используем библиотеку Natasha, которая играючи справляется со всеми базовыми задачами обработки естественного русского языка: сегментироваение на токены, морфологический анализ, лемматизация и - самое главное - извлечение именнованных сущностей. С помощью Natasha мы вытащили из датасета имена людей, названия организаций и топонимы.

Мы хотели, чтобы все элементы и все инструменты были понятны и удобны для пользователя. Поэтому уделяли особое внимание визуализации данных. Мы использовали как классические инструменты разведочного анализа данных, так и специальные интерактивные блоки для визуализации тематического моделирования (pyLDAvis) и облака слов для иллюстрации распределения именнованных сущностей.

Посмотрите, как всё это работает, в нашей [интерактивной презентации в Streamlit](https://aveletuk-deconstructing-news--streamlit-presentationpres-hlzm80.streamlitapp.com "Интерактивная презентация").

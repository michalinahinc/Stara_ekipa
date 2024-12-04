# Stara_ekipa
Analiza danych - Projekt zespołowy.

#analiza braków danych

library(naniar)
n_miss(pozyczki)
#mamy 149 braków danych

#procent braków
prop_miss(pozyczki)
#mamy 1,9% braków danych w stosunku do całości obserwacji

#tabela podsumowująca
miss_var_summary(pozyczki)
#najwięcej braków mamy w kolumnie "credit_history", ale są też kolumny, w których jest komplet danych

#wizualizacja ogólna
vis_miss(pozyczki)
#vis_miss(pozyczki, cluster=TRUE)
vis_miss(pozyczki, sort_miss=TRUE)

#mapa
gg_miss_fct(pozyczki, fct = Self_Employed)
gg_miss_fct(pozyczki, fct = Married)
gg_miss_fct(pozyczki, fct = Education)
gg_miss_fct(pozyczki, fct = Credit_History)
#Naszym zdaniem zmienna Education prezentuje największe rozbieżności pomiędzy brakami danych.





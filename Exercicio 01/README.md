select database()pokedex; <br>
show columns from pokemon;<br>
select * from pokemon;<br>
select numero,nome,cor,altura_m,peso_kg from pokemon;<br>
select numero,nome from pokemon where geracao = 1;<br>
select * from pokemon where geracao = 1 and cor = 'Amarelo';<br>
select nome,ataque from pokemon order by ataque desc LIMIT 1;<br>
select numero,nome,tipo1 from pokemon where tipo1 = 'fire';<br>
select numero,nome,defesa from pokemon order by numero desc;<br>
select numero,nome from pokemon ordeR by taxa_captura LIMIT 1;<br>
select * from pokemon where tipo2 IS NULL;<br>
select numero,nome,tipo1,tipo2 from pokemon where peso_kg between 100 and 500;<br>
select numero,nome,velocidade from pokemon order by  velocidade desc LIMIT 10;<br>
select numero,nome,tipo1,tipo2,taxa_captura from pokemon where tipo1 IS NOT NULL and tipo2 IS NOT NULL and taxa_captura >100 order by taxa_Captura desc;<br>
select distinct tipo1 from pokemon;<br>
select numero,nome,cor from pokemon where nome like 'd%';<br>
select nome,total from pokemon order by total desc limit 1;<br>
select numero,nome,defesa,ataque from pokemon where defesa>60 and ataque<=70 order by total desc;<br>
select * from pokemon where tipo1='planta' or tipo1='venenoso' and tipo2='planta' or tipo2='venenoso' and cor != 'Green' order by nome asc;<br>
select nome from pokemon where nome like '___y%';<br>
select ataque_especial from pokemon order by ataque_especial desc limit 1;<br>
select numero,nome,altura_m from pokemon where altura_m >2.10;<br>
select distinct cor from pokemon  order by cor asc;<br>
select nome,velocidade from pokemon where velocidade between 30 and 70 order by nome asc, velocidade desc;<br>
select nome,lendario from pokemon where lendario=1 order by total desc;<br>
select * from pokemon where geracao=1 and taxa_captura = 255;<br>
select nome from pokemon where nome = 'pikachu'or nome ='Squirtle' or nome='Bulbasaur' or nome= 'Charmander' order by total desc;<br>
select nome from pokemon where nome like 'd%' and geracao=1 and tipo2 IS NOT NULL order by taxa_captura asc, total desc;<br>
select numero,nome,total,taxa_captura from pokemon where lendario=1 order by taxa_captura asc, total asc;<br>
select numero,nome,peso_kg from pokemon where peso_kg between 2 and 3; <br>
select numero,nome,tipo1,tipo2 from pokemon where tipo1='normal' and tipo2 IS NULL and lendario=0;<br>
select numero,nome,tipo1,tipo2,cor from pokemon where cor !='Blue' order by nome asc;<br>
select nome,velocidade from pokemon order by velocidade asc LIMIT 10;<br>
select nome from pokemon where nome like 'a%a';<br>
select nome from pokemon where tipo1='fire' and cor !='red' order by nome asc;<br>
select distinct peso_kg from pokemon order by peso_kg asc;<br>
select numero,nome,hp from pokemon where hp between 0 and 100 order by hp,nome asc;<br>
select numero,nome,hp,ataque,defesa,total from pokemon where hp >=100 and ataque>=100 and defesa>=100; <br>
select nome,tipo1 from pokemon where tipo1='Water' or tipo1='gelo' order by total desc;<br>

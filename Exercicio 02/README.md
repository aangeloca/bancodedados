use pokedex; <br>
select max(total), min(total), max(hp),min(hp),max(ataque),min(ataque),max(defesa),min(defesa),max(ataque_especial),min(ataque_especial),max(defesa_especial),min(defesa_especial),max(velocidade),min(velocidade),max(taxa_captura),min(taxa_captura) from pokemon;<br>
select count(DISTINCT cor) from pokemon;<br>
select avg(peso_kg) from pokemon;<br>
select sum(altura_m) from pokemon;<br>
select count(*) from pokemon;<br>
select avg(altura_m) from pokemon;<br>
select std(hp) from pokemon;<br>
select count(tipo2) from pokemon;<br>
select count(DISTINCT tipo1) from pokemon;<br>
select sum(peso_kg) from pokemon;<br>
select count(lendario)from pokemon where lendario = 1 ; <br>
select count(lendario)from pokemon where lendario = 0 ; <br>
select count(*), count(DISTINCT cor) from pokemon ORDER BY COR DESC;<br>
select avg(peso_kg), avg(altura_m) from pokemon ORDER BY peso_kg, altura_m desc ;<br>
select avg(taxa_captura), cor from pokemon group by cor; <br>
select tipo1,avg(taxa_captura) as captura from pokemon group by tipo1 having captura >100;<br>
select avg(total),nome from pokemon where lendario = 0 group by cor having avg(total) <400; <br>
select max(total),geracao from pokemon group by geracao; <br>
select count(lendario),geracao from pokemon where lendario =1 group by geracao;<br>
select count(tipo1), count(tipo2), avg(taxa_captura),geracao from pokemon group by geracao ;<br>
select  count(cor),geracao from pokemon where lendario=1 group by geracao;<br>
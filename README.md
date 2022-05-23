# e-o-oscar-vai-para

Muito bem, Pessoal... 

Hoje vamos trabalhar com o Oscar.
A ideia de premiar ou ser premiado é para reconhecer:
- Reconhecer uma qualidade
- Reconhecer um atributo
- Reconhecer o esforço... 

Reconhecer sempre.

Nem todos os prêmios são merecidos e nem todos que merecem ganham. 
Então vale mesmo a pena, premiar? 


Aqui vai uma ajudinha:
Nesse exercício vamos usar alguns comandos bem básicos como 

SELECT COUNT(*) FROM tabela_exemplo WHERE coluna_exemplo = "Novo Valor";

SELECT * FROM tabela_exemplo WHERE coluna_exemplo = "Novo Valor"  AND coluna_exemplo2 = "Outro Valor";

SELECT * FROM tabela_exemplo WHERE coluna_exemplo LIKE 'eda';

UPDATE tabela_exemplo SET coluna_exemplo = "Novo Valor" WHERE id = 1;

INSERT INTO tabela_exemplo (coluna_1,, coluna_2) VALUES ("VALOR 1", "VALOR 2");


Quantas vezes Natalie Portman foi indicada ao Oscar?
R:
3 vezes
SELECT name, COUNT(*) FROM oscar WHERE name LIKE '%Natalie Portman%';


Quantos Oscars Natalie Portman ganhou?
R:
1 vez
SELECT COUNT(*) FROM oscar WHERE name LIKE '%Natalie Portman%' AND winner LIKE '%True%';


Amy Adams já ganhou algum Oscar?
R:
não
SELECT COUNT(*) FROM oscar WHERE name LIKE '%Amy Adams%' AND winner LIKE '%True%';


Alguém já ganhou um Oscar e tem o seu primeiro nome?
R:
não :(
SELECT COUNT(*) FROM oscar WHERE name LIKE '%Camily%' AND winner LIKE '%True%';


Toy Story 3 ganhou um Oscar em quais anos?
R:
2010
SELECT name, year_film FROM oscar WHERE film LIKE '%Toy Story 3%' AND winner LIKE '%True%';


Quem tem mais Oscars: a categoria "Melhor Ator" ou "Melhor Filme"?
R:
melhor ator
SELECT category, COUNT(category) FROM oscar WHERE category LIKE '%ACTOR' OR category LIKE '%CINEMATOGRAPHY' AND winner LIKE '%True%' GROUP BY category;


O primeiro Oscar para melhor Atriz foi para quem? Em que ano?
R:
Janet Gaynor	1928
SELECT name, MIN(year_ceremony) FROM oscar WHERE category LIKE '%ACTRESS%' AND winner LIKE '%True%';


Na categoria Winner, altere todos os valores com "True" para 1 e todos os valores "False" para 0.


Em qual edição do Oscar "Crash" ganhou o prêmio?


Que filme merecia ganhar um Oscar e não ganhou?


Bom... dê um Oscar para esse filme, então.



O filme Central do Brasil aparece no Oscar?



Aliás... Qual sua opinião sobre central do Brasil



Inclua no banco 7 filmes que nunca nem foram nomeados ao Oscar, mas que na sua opinião, merecem.



Crie uma nova categoria de premiação. Qualquer prêmio que você queira dar. Agora vamos dar esses prêmios aos filmes que você cadastrou na questão acima.



Qual foi o primeiro ano a ter um prêmio do Oscar?



Pensando no ano em que você nasceu: Qual foi o Oscar de melhor filme, Melhor Atriz e Melhor Diretor?



Agora procure 7 atrizes que não sejam americanas, europeias ou brasileiras.  Vamos cadastrá-los no nosso banco, mas eles ainda não ganharam o Oscar. Só foram nomeados.



Agora vamos falar da sua vida. Me diga o nome de uma pessoa que você admira e o que ela fez na sua vida. Agora me diz: Quê prêmio essa pessoa merece?



[OPCIONAL] - Utilizando o comando 'Alter Table', troque os tipos dos dados da coluna/campo "Winner" para Bit.



Eduardo Galeano.
“A utopia está lá no horizonte. Me aproximo dois passos, ela se afasta dois passos. Caminho dez passos e o horizonte corre dez passos. Por mais que eu caminhe, jamais alcançarei. Para que serve a utopia? Serve para isso: para que eu não deixe de caminhar.”

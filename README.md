# zodiac
Pretende-se fazer um programa que com base na data de nascimento e data actual determina a idade e o signo do zodiaco.
Além disso, o programa deverá também determinar se a pessoa está apta para trabalhar (idade >= 16) ou se é elegível para a reforma (idade >= 66 anos e 5 meses) 


## Descrição do problema
O programa recebe um caracter e 6 inteiros. O caracter serve para escolher qual o output a apresentar:
    - 'a' - idadade
    - 'z' - signo do zodiaco
    - 'r' - informação sobre se está apto para trabalhar ou elegível para a reforma
    - 't' - toda a informação
Os 6 inteiros correspondem a dia, mês e ano de nascimento e dia, mês e ano atual

Exemplo:
```bash
a 05 08 2015 01 01 2020
```

### Opção 'a'
O programa deverá devolver a idade do utilizador
Exemplo:
```bash
a 05 08 2015 01 01 2020
4 anos
```
### Opção 'z'
O programa deverá devolver o signo do zodiaco (Capricornio, Aquario, Peixes, Carneiro, Touro, Gemeos, Carangueijo, Leao, Virgem, Balanca, Escorpiao, Sagitario).

Exemplo:
```bash
z 05 08 2015 01 01 2020
Leao
```

A determinação do signo deverá ser feita de acordo com as seguintes datas:
    - Capricornio - Dec 22 a Jan 19
    - Aquario - Jan 20 a Feb 18
    - Peixes - Feb 19 a Mar 20
    - Carneiro - Mar 21 a Apr 19
    - Touro - Apr 20 a May 20
    - Gemeos - May 21 a Jun 20
    - Carangueijo - Jun 21 a Jul 22
    - Leao - Jul 23 a Aug 22
    - Virgem - Aug 23 a Sep 22
    - Balanca - Sep 23 a Oct 22
    - Escorpiao - Oct 23 a Nov 21
    - Sagitario - Nov 22 a Dec 21 

### Opção 'r'
Consoante a idade, o programa deverá mostrar uma das seguintes mensagens
```
Apto para trabalhar
```
ou
```
Nao tem idade para trabalhar
```
ou
```
Elegivel para reforma
```
A idade mínima para se considerar Apto para trabalhar é de 16 anos e a idade mínima para se estar elegível para a reforma é de idade >= 66 anos e 5 meses.

Exemplo:
```bash
z 05 08 2015 01 01 2020
Nao tem idade para trabalhar
```

### Opção 't'
O programa deverá mostrar toda a informação. Exemplo:
Exemplo:
```bash
z 05 08 2015 01 01 2020
4 years old
Leo
Nao tem idade para trabalhar
```

## Mensagens de erro
Se o utilizador introduzir uma data de nascimento inválida o programa deverá responder
"Data de nascimento invalida".

Se o utilizador introduzir a data atual inválida o programa deverá responder "Data actual invalida".

Nota: considera-se ano inválido se for inferior a 1900 ou superior a 2020. Considera-se o dia
inválido se for menor que 1 ou superior ao numero máximo de dias de cada mês.

O programa deverá também validar as datas relativamente aos dias de cada mês e especialmente em relação aos dias do mês de fevereiro. Para isso deverá tomar em consideração se o no é bissexto ou não.

O programa deverá sempre validar datas antes de qualquer outra operação. 

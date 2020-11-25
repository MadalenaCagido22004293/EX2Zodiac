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
a 11 1 1970 2 6 2020
50 anos
```
### Opção 'z'
O programa deverá devolver o signo do zodiaco (Capricornio, Aquario, Peixes, Carneiro, Touro, Gemeos, Carangueijo, Leao, Virgem, Balanca, Escorpiao, Sagitario).

Exemplo:
```bash
z 18 02 1930 12 10 2020
Aquario
```

A determinação do signo deverá ser feita de acordo com as seguintes datas:
- Capricornio - Dec 22 a Jan 19
- Aquario - Jan 20 a Feb 18
- Peixes - Feb 19 a Mar 20
- Carneiro - Mar 21 a Apr 19
- Touro - Apr 20 a May 20
- Gemeos - May 21 a Jun 2r
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
r 01 01 1999 01 01 2020
Apto para trabalhar
```

### Opção 't'
O programa deverá mostrar toda a informação. Exemplo:
Exemplo:
```bash
t 13 5 1967 30 9 2020
53 anos
Touro
Apto para trabalhar
```

## Mensagens de erro
Se o utilizador introduzir uma data de nascimento inválida o programa deverá responder
"Data de nascimento invalida".

Se o utilizador introduzir a data atual inválida o programa deverá responder "Data actual invalida".

Nota: considera-se ano inválido se for inferior a 1900 ou superior a 2020. Considera-se o dia
inválido se for menor que 1 ou superior ao numero máximo de dias de cada mês.

O programa deverá também validar as datas relativamente aos dias de cada mês e especialmente em relação aos dias do mês de fevereiro. Para isso deverá tomar em consideração se o no é bissexto ou não.

Se o utilizador introduzir uma data actual inferior à data de nascimento, o programa deverá imprimir a mensagem ```Data actual inferior a data de nascimento```.

O programa deverá sempre validar datas antes de qualquer outra operação. 

# Entrega
O programa deverá ser submetido na plataforma PANDORA [(2)](#ref2) até às *23:59 do dia 27/11/2020*. O desenvolvimento do programa deverá ser realizado individualmente. 

## Honestidade Académica

Nesta disciplina, espera-se que cada aluno siga os mais altos padrões de honestidade académica. Trabalhos que sejam identificados como cópias serão anulados e os alunos envolvidos terão nota zero - quer tenham copiado, quer tenham deixado copiar.
Para evitar situações deste género, recomendamos aos alunos que nunca partilhem ou mostrem o seu código.
A decisão sobre se um trabalho é uma cópia cabe exclusivamente aos docentes da unidade curricular.
Os alunos são encorajados a discutir os problemas com outros alunos mas não deverão, no entanto, copiar códigos, documentação e relatórios de outros alunos. Em nenhuma circunstância deverão partilhar os seus próprios códigos, documentação e relatórios. De facto, não devem sequer deixar códigos, documentação e relatórios em computadores de uso partilhado.

*Todos os entregues serão comparados utilizando um algoritmo de detecção de plágio [(3)](#ref3) que automaticamente atribui uma percentagem de semelhança entre os trabalhos. Este algoritmo é extremamente robusto e será utilizado nesta disciplina em todos os trabalhos ao longo do ano.* 

## Referências

<a name="ref1"></a>

* (1) Pereira, A. (2017). C e Algoritmos, 2ª edição. Sílabo.

<a name="ref2"></a>

* (2)  PANDORA - Yet Another Automated Assessment Tool, https://saturn.ulusofona.pt/.

<a name="ref3"></a>

* (3)  Saul Schleimer, Daniel S. Wilkerson, and Alex Aiken. 2003. Winnowing: local algorithms for document fingerprinting. In Proceedings of the 2003 ACM SIGMOD international conference on Management of data (SIGMOD '03). Association for Computing Machinery, New York, NY, USA, 76–85. DOI:https://doi.org/10.1145/872757.872770

## Metadados

* Autor: [Pedro Serra]
* Instituição: [Universidade Lusófona de Humanidades e Tecnologias][ULHT]



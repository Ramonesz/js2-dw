etapa 5

1
a media e 6 875

porque 8 mais 6 5 mais 9 mais 4 da 27 5 e dividindo por 4 notas da 6 875

2
o indice do primeiro elemento e 0

o indice do ultimo e length menos 1

3
for (let i = 2; i <= 10; i += 2) {
  console.log(i);
}

4
total começa com 0

volta 1 i vale 1 total fica 1
volta 2 i vale 2 total fica 3
volta 3 i vale 3 total fica 6
volta 4 i vale 4 total fica 10

sera impresso 10

etapa 6

1
imprime undefined

o erro e que a funcao faz a conta a mais b mas nao tem return entao nao devolve nada

para corrigir e so escrever return a + b

2
function ehPar(n) {
  return n % 2 === 0;
}

3
console.log mostra o valor no console so para a gente ver mas a funcao nao devolve nada

return devolve o valor para quem chamou a funcao e encerra ela entao o resultado pode ser guardado em variavel ou usado em outras contas

etapa 7

1
aparece o erro TypeError cannot set properties of null

isso acontece porque sem o defer o script roda antes do navegador ler o html entao o getElementById nao encontra o elemento e devolve null e nao da para mudar o textContent de null

2
a cada clique o navegador executa a funcao do addEventListener

a variavel cliques soma 1 com cliques++

depois o textContent do span contador recebe o novo valor de cliques e o numero na tela sobe

3
porque o valor de cliques muda a cada clique e const nao pode ser reatribuido entao daria erro de assignment to constant variable

etapa 8

8 3

function calcularMedia(n1, n2) {
  return (n1 + n2) / 2;
}

1
porque a divisao tem prioridade e n1 + n2 / 2 divide so o n2 por 2 e depois soma com n1

com 8 e 6 dá 8 + 3 que e 11 ja a media correta e 8 mais 6 dividido por 2 que da 7

8 4

function notaValida(n) {
  return !Number.isNaN(n) && n >= 0 && n <= 10;
}

8 5


if (texto1 === "" || texto2 === "" || !notaValida(n1) || !notaValida(n2)) {
  resultado.textContent = "Informe duas notas entre 0 e 10.";
  return;
}

const media = calcularMedia(n1, n2);
let situacao;
if (media >= NOTA_MINIMA) {
  situacao = "Aprovado";
} else {
  situacao = "Abaixo da média";
}
resultado.textContent = `Média: ${media.toFixed(1)} - ${situacao}`;

8 6

8 e 7 da media 7 5 aprovado

5 e 6 da media 5 5 abaixo da media

6 e 6 da media 6 0 aprovado no limite

10 e 10 da media 10 0 aprovado

vazio e 5 mensagem de erro

11 e 5 mensagem de erro

checkpoint

1
porque assim o calculo fica separado e organizado e pode ser testado sozinho no console e reaproveitado em outros lugares sem copiar o codigo

2
so uma linha porque o valor fica guardado na constante NOTA_MINIMA e o resto do codigo usa o nome dela entao basta trocar o 6 por 7 la em cima

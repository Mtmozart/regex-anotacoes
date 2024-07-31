![Imagem com texto Curso de Expressões regulares](assets/Programação-Regex.png "Title")

# Curso Alura - Expressões Regulares

Este repositório contém material do curso sobre Expressões Regulares. As expressões regulares, frequentemente chamadas de "regex" ou "regexp", são poderosas ferramentas para busca, validação e manipulação de texto. Este curso visa fornecer uma introdução abrangente e prática ao mundo das expressões regulares.

## Como Usar

Clone este repositório para sua máquina local:

```shell
git clone https://github.com/camilapessoa/regex_curso.git
```

## Ferramentas

- Node.js
- Google Collab python
- JavaScript
- HTML
- CSS

## Notas do estudante sobre regex:

- Regex são uma sequência de caracteres que ajudam a identificar outros caracteres,

\*\* GREP - GLOBAL REGULAR EXPRESSION PRINT

O grep funciona com um patten que é a expressão regular e o target que é o alvo, onde vamos encontrar que são processados pela Regex Engineer que está presente em Java, C#, Python, C etc...

- Pode fazer pesquisa de regex no termina do linux com o comando grep "expressão" "caminho"
- Com flags grep -n "expressão" "caminho" = retorna o número

** Outro caminho **
Claro! Aqui está a versão sem formatação de terminal:

---

### Comandos `grep`

- **`grep -i` ou `--ignore-case`**: Ignora a diferenciação entre maiúsculas e minúsculas, tornando a pesquisa insensível a letras maiúsculas ou minúsculas.  
  `grep -i "padrão" arquivo.txt`

- **`grep -v` ou `--invert-match`**: Inverte a correspondência, exibindo linhas que não contêm o padrão especificado.  
  `grep -v "padrão" arquivo.txt`

- **`grep -r` ou `-R` ou `--recursive`**: Realiza uma pesquisa recursiva em diretórios e seus subdiretórios. Útil para encontrar padrões em árvores inteiras de diretórios.  
  `grep -r "padrão" /caminho/do/diretório`

- **`grep -l` ou `--files-with-matches`**: Exibe apenas os nomes dos arquivos que contêm correspondências, em vez das próprias linhas correspondentes.  
  `grep -l "padrão" *`

- **`grep -c` ou `--count`**: Exibe apenas o número de correspondências em cada arquivo, em vez das próprias linhas correspondentes.  
  `grep -c "padrão" arquivo.txt`

- **`grep -n` ou `--line-number`**: Exibe o número da linha junto com as linhas correspondentes.  
  `grep -n "padrão" arquivo.txt`

- **`grep -E` ou `--extended-regexp`**: Interpreta o padrão de pesquisa como uma expressão regular estendida (Regex) em vez de uma correspondência literal.  
  `grep -E "padrão1|padrão2" arquivo.txt`

- **`grep -f <arquivo>` ou `--file=<arquivo>`**: Lê os padrões de pesquisa de um arquivo em vez de especificá-los diretamente na linha de comando.  
  `grep -f padrões.txt arquivo.txt`

- **`grep -h` ou `--no-filename`**: Suprime a exibição dos nomes dos arquivos ao imprimir as linhas correspondentes.  
  `grep -h "padrão" *`

- **`grep -P`**: Habilita o modo de interpretação de padrões como expressões regulares Perl (Perl-Compatible Regular Expressions ou PCRE). Isso significa que você pode usar padrões de expressões regulares mais avançados e complexos com a flag `-P`. As expressões regulares Perl são mais poderosas e flexíveis do que as expressões regulares básicas usadas pelo `grep` por padrão. No entanto, nem todas as versões do `grep` suportam a opção `-P`, pois ela depende da biblioteca PCRE (Perl-Compatible Regular Expressions). Portanto, verifique a disponibilidade dessa opção na versão específica do `grep` em seu sistema.  
  `grep -P "padrão\w+" arquivo.txt`

- **`man grep`**: Apresenta toda a documentação do `grep` no terminal.  
  `man grep`

---

## Meta-char

- / regex / = início e fim da regex;
- d = dígitos de 0 a 9;
- s = espaço vazio;
- g = aplicação de toda as ocorrências no artigo;
- gm = flag de busca globa com multilinhas
- \ \ = permite usar outros caracteres como o ();
- {2} = quantidades de dígitos;
- [classe onde posso por caracteres] = entre colchetes eu posso passar vários meta chars;
- ? = Quantificador que torna tudo opcional.
- $ = ancora que será no final da linha
- ^ = ancora que será no início da linha

### Regex em javascript

Para verificar se uma expressão regular corresponde a uma string e encontrar todas as correspondências, você pode usar o método `variável.match(regexCriada)`. Esse método retorna um array contendo todas as correspondências encontradas na string para a expressão regular fornecida. Se não houver nenhuma correspondência, o resultado será `null`.

Classificação segundo a Alura:
Regex Descrição Correspondência
[a-z] Qualquer letra minúscula de 'a' a 'z' "a", "m", "z"
[0-9] Qualquer dígito de 0 a 9 "0", "7", "9"
[A-Za-z] Qualquer letra maiúscula ou minúscula "A", "b", "Z"
[0-9A-Fa-f] Qualquer caractere hexadecimal "1", "A", "d"
[^0-9] Qualquer caractere que não seja um dígito "a", "B", "!"
[aeiou] Qualquer vogal minúscula "a", "e", "o"
[^aeiou] Qualquer caractere que não seja uma vogal "b", "z", "1"
[|?/’] Caracteres literais "|", "/", " ? ", “‘”

Caractere Descrição

- Hífen usado para definir intervalos de caracteres. Pode ser escapado com \ para ser tratado como um literal.
  ] Colchete de fechamento usado para marcar o fim de uma classe de caracteres. Pode ser escapado com \ para ser tratado como um literal.
  ^ Circunflexo usado para negar uma classe de caracteres quando colocado no início de [ ]. Dentro de [ ], é tratado como um literal.
  \ Barra invertida usada para escapar caracteres especiais dentro de [ ] para que sejam tratados como literais.

  Atalhos shorthands
  Regex Descrição Correspondência
  \d Qualquer dígito decimal "0", "7", "9"
  \D Qualquer caractere que não seja um dígito "a", "B", "!"
  \w Qualquer caractere alfanumérico "A", "b", "0"
  \W Qualquer caractere que não seja alfanumérico "!", "@", " "
  \s Qualquer caractere de espaço em branco " ", "\t", "\n"
  \S Qualquer caractere que não seja espaço em branco "a", "B", "9"
  \b Croa um limite para pesquisa, boa para regex específica

  Regex Descrição Correspondência
  \[ Colchete de abertura [ literal "["
  \] Colchete de fechamento ] literal "]"
  \. Ponto . literal "."
  \+ Sinal de adição + literal "+"
  \\ Escape \ literal ""

```Javascript
const texto = "Algum texto bem interessante";
const regexCriada = /interessante/;
const resultado = texto.match(regexCriada);
console.log(resultado); // ["interessante"]
```

** Atenção **, se for procurar regex em arquivos, adicione o "g" no fim da regex.

-- Telefone tipo **`/\(\d{2}\)\s\d{4,5}-\d{4}/`** = **`(dd) 9999-99999`**

-- CPF tipo **`/\d{3}\.\d{3}\.\d{3}\-\d{2}/`** = **`123.456.789-10`**

-- Data tipo **`/\d{2}\/\d{2}\/\d{4}/`** = **`05/08/1998`**

-- Nome válido **`/^[A-Za-zÀ-ÿ -]{3,30}$/i`** = **Só um nome**

-- Nome válido **`/^(?!(.)\1\1)[A-Za-zÀ-ÿ -]{3,30}$/i`** = **Só um nome, só que mais restrito**

-- Endereço **`/[A-Za-zÀ-ÿ -]+,\s\d{3}+,\sCEP\s\d{5}-\d{3}/gm`** = **/[A-Za-zÀ-ÿ -]+,\s\d{3}+,\sCEP\s\d{5}-\d{3}/**

## Conceitos importantes:

Vamos usar a analogia da biblioteca para entender o que fizemos na aula:A nossa "biblioteca" é o código HTML da página do MoniBank. Nesse código, temos várias tags, como <h1>, <h2>, <p>, e outras.O nosso "livro" é o conteúdo dentro de cada tag. Por exemplo, dentro da tag <h1> está o título da página "MoniBank".A nossa "busca" é encontrar todas as tags <h1> e <h2> e seus conteúdos.No início, nossa regex era greedy: Ela "pegava todos os livros da estante", ou seja, capturava todo o conteúdo do HTML até encontrar a próxima tag de fechamento </h1> ou <h2>. Isso incluía espaços em branco e o conteúdo de outras tags, como <p>, que não eram relevantes para a nossa busca.Para resolver esse problema, usamos o quantificador lazy \*?: Ele "olhava rapidamente para os livros da estante" e pegava apenas o primeiro livro que encontrava, ou seja, o conteúdo da tag <h1> ou <h2> até a próxima tag de fechamento. Assim, nossa regex se tornou mais precisa e eficiente, capturando apenas o conteúdo que realmente queríamos.Você pode pensar na regex como um detetive que procura pistas em um crime. Um detetive greedy vai analisar todos os detalhes, mesmo os irrelevantes, enquanto um detetive lazy vai focar nas pistas mais importantes.Espero que essa analogia tenha te ajudado a entender como greedy e lazy funcionam na prática! Você tem alguma outra dúvida sobre a aula?

## outro dicionário importante:

    Descrição	Exemplo

- Coincide com 0 ou mais ocorrências do elemento anterior. a\* corresponde a "", "a", "aa", "aaa", etc.

* Coincide com 1 ou mais ocorrências do elemento anterior. a+ corresponde a "a", "aa", "aaa", etc., mas não a "".
  ? Coincide com 0 ou 1 ocorrência do elemento anterior. a? corresponde a "" ou "a".
  {n} Coincide exatamente com “n” ocorrências do elemento anterior. a{3} corresponde a "aaa", mas não a "aa" ou "a".
  {n,} Coincide com pelo menos “n” ocorrências do elemento anterior. a{2,} corresponde a "aa", "aaa", "aaaa", etc.
  {n,m} Coincide com pelo menos “n” e no máximo “m” ocorrências do elemento anterior.

notas: é como um "espelho" dentro da sua regex, que permite você referenciar um grupo de captura anterior dentro da mesma expressão.

Imagine que você está procurando por um padrão de texto onde a primeira parte precisa ser exatamente igual à última parte. Por exemplo, você quer encontrar todas as tags HTML que abrem e fecham com o mesmo nome, como <h1 ... </h1> ou <p ... </p>.

Com backreference, você pode capturar a primeira parte da tag (o nome da tag) e depois usar essa captura para garantir que a última parte seja exatamente igual.

Exemplo:
python

```python
pattern = r'<(h[12])[^>]_>(._?)<\/\1>'
```

Nesse exemplo, o grupo (h[12]) captura a primeira parte da tag (h1 ou h2). O \1 é a backreference que faz referência ao primeiro grupo capturado, garantindo que a tag de fechamento seja exatamente igual à de abertura.

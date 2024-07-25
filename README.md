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

Você pode copiar e colar diretamente no seu README agora!

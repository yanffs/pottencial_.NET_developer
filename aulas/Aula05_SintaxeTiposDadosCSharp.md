# Sintaxe Convenções

Para criar um novo projeto pode utilizar a função no terminal: *dotnet new console*

## Arquivos

Tipos de arquivos ao criar um projeto em C#

- .cs -> Que faz a codificação no C#
- .csproj -> linguagem xml, que está relacionado ao seu projeto, isto é, informações da base do projeto, como no caso do R studio  (Metadados)
  - Mostra informações relacionadas ao projeto como deve se comportar e não existe necesidade de modificá-lo
- Pasta **obj** - arquivos de *debug*
- Pasta **bin** - arquivos *binários*
Uma estrutura de projeto em C# é composto por basicamente por essas estruturas

## Conceito de classes
**O que é uma classse?** é um Tipo abstrato de Dados (TAD); ou seja, uma descrição que abstrai um conjunto de objetos com características similares (um projeto do objeto), é um código da linguagem de programação orientada a objetos que define e implementa um novo tipo de objeto, que terão características (atributos) que guardaram valores e, também funções específicas para manipular estes.
- Ela representa a construção de um objeto, isto é, apenas informações necessárias que caracterizam um objeto específico

## Criando nossa classe no código
Criando um novo arquivo no projeto
- No vscode:
  - Explorer + botão direito do mouse + nova pasta + new C# + class - Primeira convenção do C# todo nome de classe deve começar com maiúsculo e a cada nova palavra deve começar também com letra maiúscula, por exemplo: **PessoaFisica**, que seria **Pessoa Física**
  - Irá digitar prop e tab para escolher a melhor versão para o seu caso
    - Texto é apotando, como **string** para o C#. Cadeia de caracteres

## Entendendo a estrutura do código
- Get -> pega valor
- Set -> Atribui o valor
- Diferenças entre classes e métodos
  - Classe em verde (não possui parênteses)
  - Método/função em amarelo (possi parênteses)
  - Argumentos em laranja (geralmente está dentro dos parênteses)
- Palavras proibida - são palavras proibidas de usá-las pelo C#, pois já estão reservadas para serem utilizadas, como palavras padrão pelo C#. Uma alternativa é colocar o @ na frente da palavra reservada/proibida. Mas aumenta a chance de erros/aumenta a complexidade.
- Exemplos de palavras reservadas: get, set, class, int, string e assim por diante

## Usando namespaces
Todas as nossas alterações devem partir do arquivo "Program.cs", desta forma devemos atribuir as funções a partir dele
- Quando estiver se referindo a uma classe contida em uma outra pasta utilizar sempre a função/método **using** e o caminho para o arquivo, por exemplo:
  -  **using fundamentos.Models;**

## Utilizando a classe pessoa
Exemplo prático não necessita de anotações aqui
## Explorando a sintaxe
- Todo comando tem que ser acompanhado de ponto e vírugla
- O ponto apresenta tudo o que eu posso mudar com o meu objeto, por exemplo, aqui para a pessoa 1 identificada lá em cima eu vou atribuir a idade 26
  - pessoa1.Idade = 26;
- Para fazer a quebra de linha é simples, por exemplo:
  - **Console.WriteLine($"Olá, meu nome é {Nome}, e tenho {Idade} anos");** - É sem a quebra de linha para adicioná-la basta:
    - Console.WriteLine($"Olá, meu nome é {Nome},"+
    - "e tenho {Idade} anos");
  - **Ou seja,** basta fechar a string com aspas dar enter e colocar um sinal de adição "+", após o fechamento da string e abrir a string na linha seguinte
  - Caso queira quebrar a linha do texto que será retornado com o comando, basta adicionar um "**\n**", isto é, quebra de linha

## Convenções case
Não são obrigatórias, mas por questões repetibilidade são seguidas pelo usuários a fim de facilitar o compartilhamento de códigos
- Existe alguns tipos de convençõe de acordo com a escrita dos objetivos. Mais conhecidas, como cases, sendo elas
  - **camelCase** - incial minúscula a cada nova palavra a incial será colocada em maiúsculo
  - **PascalCase** - inicial maiúsucla e a cada nova palavra a incial também será colocada em maiúscula
  - **snake_case** - tudo minúsculo com as novas palavras separadas por underscore
  - **spinal-case** - tudo minúsuclo com as novas palavras separadas por hífen

## Convenções case no código
Aplicações
- Nome de classe sempre será utilizado o **PascalCase**
- Nome de propriedade sempre será utilizado o **PascalCase**
- Nome de método/função sempre será utilizado o **PascalCase**
- Nome de varíavel sempre será utilizado o **camelCase**

## Convenções escrita de classe
A recomendação é que nunca seja abreviado

## Convenção de nome e variável
Não pode haver caracter especial em nome de variável e por ai vai

# Ontologia de Atores

Esta ontologia foi desenvolvida para representar informações relacionadas a atores, suas carreiras, personagens interpretados, prêmios recebidos e colaborações com diretores. Utilizando a linguagem OWL2, a ontologia oferece uma estrutura para representar informações sobre atores e suas atividades na indústria do entretenimento. A seguir, são apresentados os principais elementos da ontologia:

## Classes:

1. **Ator:**
   - Representa um ator na ontologia.
   - Propriedades:
     - `nome` (Propriedade de Dados): Nome do ator.
     - `dataNascimento` (Propriedade de Dados): Data de nascimento do ator.
     - `nacionalidade` (Propriedade de Dados): Nacionalidade do ator.
     - `atuouEm` (Propriedade de Objeto): Relaciona o ator a filmes ou séries em que atuou.
     - `recebeuPremiacao` (Propriedade de Objeto): Relaciona o ator a prêmios que recebeu.

2. **Carreira:**
   - Representa a carreira de um ator.
   - Subclasse de: `owl:Thing`.
   - Propriedades:
     - `atuouEm` (Propriedade de Objeto): Lista de filmes e séries em que o ator participou.

3. **Personagem:**
   - Representa um personagem interpretado por um ator.
   - Propriedades:
     - `nomePersonagem` (Propriedade de Dados): Nome do personagem.
     - `generoPersonagem` (Propriedade de Dados): Gênero do personagem (drama, comédia, etc.).
     - `anoInterpretacao` (Propriedade de Dados): Ano em que o ator interpretou o personagem.

4. **Diretor:**
   - Representa um diretor com quem um ator colaborou.
   - Propriedades:
     - `colaborouCom` (Propriedade de Objeto): Lista de diretores com quem o ator colaborou.

5. **Premiacao:**
   - Representa uma premiação recebida por um ator.
   - Propriedades:
     - `nomePremiacao` (Propriedade de Dados): Nome da premiação.
     - `anoPremiacao` (Propriedade de Dados): Ano em que o prêmio foi concedido.

6. **EstiloAtuacao:**
   - Representa o estilo de atuação preferido ou característico de um ator.
   - Subclasse de: `owl:Thing`.

7. **Filme:**
   - Representa um filme na ontologia.
   - Subclasse de: `owl:Thing`.
   - Propriedades:
     - `nome` (Propriedade de Dados): Nome do filme.

8. **CategoriaPremiacao:**
   - Representa uma categoria de premiação.
   - Subclasse de: `owl:Thing`.
   - Propriedades:
     - `nome` (Propriedade de Dados): Nome da categoria.

## Propriedades:

1. **Propriedades de Objeto:**
   - `atuouEm`: Relaciona um ator a um filme ou série.
   - `interpretouPersonagem`: Relaciona um ator a um personagem específico.
   - `recebeuPremiacao`: Relaciona um ator a uma premiação específica.
   - `colaborouCom`: Relaciona um ator a diretores com quem colaborou.

2. **Propriedades de Dados:**
   - `nome`: Armazena o nome de um ator, filme, categoria de premiação, etc.
   - `dataNascimento`: Armazena a data de nascimento de um ator.
   - `nacionalidade`: Armazena a nacionalidade de um ator.
   - `nomePersonagem`: Armazena o nome de um personagem.
   - `generoPersonagem`: Armazena o gênero de um personagem.
   - `anoInterpretacao`: Armazena o ano em que um ator interpretou um personagem.
   - `nomePremiacao`: Armazena o nome de uma premiação.
   - `anoPremiacao`: Armazena o ano em que uma premiação ocorreu.

## Restrições:

1. **Restrição de Propriedade:**
   - `anoPremiacao`: Restrição que especifica que os valores desta propriedade devem ser do tipo `xsd:gYear`.


**Autores:**
- Ana Livia
- Caio

Alunos de Sistemas de Informação da UTFPR (Universidade Tecnológica Federal do Paraná).


<!-- antes de enviar a versão final, solicitamos que todos os comentários, colocados para orientação ao aluno, sejam removidos do arquivo -->

# Analise-de-similaridade-de-Banco-de-Perguntas-por-metodos-NLP

#### Aluno: [Mauro Jaimovich](https://github.com/link_do_github).
#### Orientador: [Felipe Borges](https://github.com/link_do_github).

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

- [Link para o código](https://github.com/link_do_repositorio/nome_do_arquivo_de_codigo). <!-- caso não aplicável, remover esta linha -->

- [Link para a monografia](https://link_da_monografia.com). <!-- caso não aplicável, remover esta linha -->

- Trabalhos relacionados: <!-- caso não aplicável, remover estas linhas -->
    - [Nome do Trabalho 1](https://link_do_trabalho.com).
    - [Nome do Trabalho 2](https://link_do_trabalho.com).

---

### Resumo

<!-- trocar o texto abaixo pelo resumo do trabalho, em português -->

A Proposta deste projeto é de encontrar Similaridade entre perguntas cadastradas em Banco de dados para evitar duplicidade de conteúdo, otimizando a contextualização do banco para utilização de usuários ou demandantes de informação.
Na primeira parte e na segunda parte do código houve a codificação das perguntas em Tokens numéricos e a abordagem nas duas partes foi a de comparação
por diferença entre os cossenos.
A primeira parte do código apresenta a solução de identificação de similaridade com a abordagem em Bag of Words, quando identificamos pares de perguntas
similares.
a segunda parte do código apresenta a identificação de similaridade utilizando modelos de transformação, no caso o BERT e a terceira, ou extensão da segunda
parte um modelo do tipo Electra.
Quando utilizamos a segunda parte do código e incluimos perguntas referentes aos pares identificados na parte 1, conseguimos identificar as mesmas perguntas
identificadas pelos pares, com ranqueamento por utilização de métricas dos cossenos.
O código apresentado estrutura inicialmente todas as etapas de pre processamento necessárias e que deverão ser aplicadas, independente de qual modelo . Estabelecer as etapas de transformação em caixa baixa, retirar stopwords, caracteres especiais e etc.Em seguida utilizaremos ainda neste Notebook o método de comparação por bag of words, calculando os vetores das perguntas, limitando o número de linhas, considerando a limitação de recursos computacionais do Colab. A opção então foi de não importar todas as linhas do Banco de perguntas proposto, continha 170000 perguntas e apenas buscar similaridades com as primeiras 5000 perguntas. 
O resultado para apenas 5000 perguntas , no caso de Bag of Words foi encorajador para propor a mesma busca no restante do banco de dados original que contem
170000 perguntas, uma vez que foram identificados 550 pares de perguntas com similiaridade entre cossenos maior do que 0.99.
Podemos assim indicar o método utilizado para identificar em outros bancos de dados que contenham texto a identificação de similaridades, possibilitando a exclusão direcionada pelos resultados das comparações e reduzindo duplicidades nos contextos linguísticos.



### Abstract <!-- Opcional! Caso não aplicável, remover esta seção -->

<!-- trocar o texto abaixo pelo resumo do trabalho, em inglês -->



---

Matrícula: 192671078

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*






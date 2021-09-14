<!-- antes de enviar a versão final, solicitamos que todos os comentários, colocados para orientação ao aluno, sejam removidos do arquivo -->

# Analise-de-similaridade-de-Banco-de-Perguntas-por-metodos-NLP

#### Aluno: [Mauro Jaimovich](https://github.com/jaimovi/).
#### Orientador: [Felipe Borges](https://github.com/FelipeBorgesC).

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

- [Link para o código](https://github.com/jaimovi/Analise-de-similaridade-de-Banco-de-Perguntas-por-metodos-NLP/blob/main/Perguntas_ver1.ipynb). <!-- caso não aplicável, remover esta linha -->


- Trabalhos relacionados: <!-- caso não aplicável, remover estas linhas -->
    - NLP | How tokenizing text, sentence, words works.(https://www.geeksforgeeks.org/nlp-how-tokenizing-text-sentence-words-works/).
    - BERT LaBSE Sentence Embeddings.(https://nlp.johnsnowlabs.com/2020/09/23/labse.html).

---

### Resumo


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

The purpose of this project is to find Similarity between questions registered in the Database to avoid duplication of content, optimizing the context of the database for use by users or information demanders. In the first part and in the second part of the code, the questions were encoded in numeric Tokens and the approach in both parts was the comparison by difference between the cosines. The first part of the code presents the similarity identification solution with the approach in Bag of Words, when we identify pairs of similar questions. the second part of the code presents the identification of similarity using transformation models, in this case the BERT and the third, or extension of the second part, an Electra type model. When we used the second part of the code and included questions referring to the pairs identified in part 1, we were able to identify the same questions identified by the pairs, ranked by using cosine metrics. The code presented initially structures all the necessary pre-processing steps that must be applied, regardless of which model. Establish the transformation steps in lower case, remove stopwords, special characters, etc. Then, in this Notebook, we will still use the bag of words method of comparison, calculating the question vectors, limiting the number of lines, considering the limitation of computational resources of Collabory The option then was not to import all the lines of the proposed Question Bank, it contained 170,000 questions and just look for similarities within the first 5000 questions. The result for only 5000 questions in the case of Bag of Words was encouraging to propose the same search in the rest of the original database which contains 170000 questions, since 550 pairs of questions with similarity between cosines greater than 0.99 were identified. We can thus indicate the method used to identify in other databases that contain text the identification of similarities, enabling the exclusion driven by the results of comparisons and reducing duplication in linguistic contexts.



---

Matrícula: 192671078

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*






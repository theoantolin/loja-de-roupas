# Plano de Testes de Software

Este plano de testes tem como objetivo listar os testes que serão executados com os requisitos selecionados do Sistema Web para a Loja de Roupas Bruthelu. Após a execução dos casos de teste, será feito a descrição das estratégias a serem empregadas, a identificação dos recursos necessários e disponibilização de uma estimativa dos esforços de teste.

## Diagrama de Caso de Uso - UML

O cenário escolhido para representar o plano de testes do software em desenvolvimento está descrito na imagem abaixo.

![Diagrama de caso de uso](img/diagrama-caso-uso.png)

Figura 01 - Diagrama de caso de uso

## Tabelas dos Requisitos Selecionados

**Caso de Teste** | **CT01 - Criar conta após preencher formulário**
 :--------------: | ------------
**Pré-Condição**  | Acessar a tela cadastro.
**Procedimento**  | 1) O ator preenche os campos solicitados do formulário e clica<br>no botão "Enviar".<br>2) O serviço de autenticação verifica se os dados inseridos<br>são válidos, caso não sejam, o ator deve preencher novamente<br>os campos inválidos e enviar o formulário.<br>3) O serviço de autenticação interage com o LocalStorage<br>com o objetivo de armazenar os dados ator.<br>4) O sistema mostra mensagem para o ator que o cadastro<br>foi concluído.<br>5) O ator é redirecionado para a página inicial.
**Resultado esperado** | Conseguir criar conta no site.
**Dados de entrada** | Inserção de dados válidos no formulário de cadastro.
**Prioridade**    | Alta.
**Ambiente**      | Microsoft Windows 10 Pro 21H1 19043.1081, Google Chrome<br>Versão 91.0.4472.114 (Versão oficial) 64 bits.
**Técnica**       | Manual.
**Iteração**      | 1a Iteração.

**Caso de Teste** | **CT02 - Fazer Log In em conta criada**
 :--------------: | ------------
**Pré-Condição**  | Acessar a tela conta.
**Procedimento**  | 1) O ator preenche os campos solicitados do formulário e clica<br>no botão "Entrar".<br>2) O serviço de autenticação verifica se os dados inseridos<br>são válidos, caso não sejam, o ator deve preencher novamente<br>os campos inválidos e enviar o formulário.<br>3) O ator pode selecionar a caixa checkbox "Lembre de mim",<br>que tem a função de manter o ator logado em sua conta,<br>mesmo após fechar o navegador.<br>4) O serviço de autenticação interage com o LocalStorage<br>com o objetivo de verificar os dados ator.<br>5) O ator é redirecionado para a página inicial logado em sua<br>conta.
**Resultado esperado** | Fazer log in em conta no site.
**Dados de entrada** | Inserção de dados válidos nos campos de log in.
**Prioridade**    | Alta.
**Ambiente**      | Microsoft Windows 10 Pro 21H1 19043.1081, Google Chrome<br>Versão 91.0.4472.114 (Versão oficial) 64 bits.
**Técnica**       | Manual.
**Iteração**      | 1a Iteração.
 
**Caso de Teste** | **CT03 - Procurar produto em caixa de pesquisa**
 :--------------: | ------------
**Pré-Condição**  | Acessar tela do sistema com barra de navegação.
**Procedimento**  | 1) O ator digita na caixa de pesquisa, localizada na barra de<br>navegação, o nome do produto.<br>2) O ator deve clicar no botão de lupa para efetuar a pesquisa.<br>3) O LocalStorage vai verificar se o produto pesquisado existe<br>no banco de dados.<br>4) O ator é redirecionado para a página inicial.<br>5) O sistema exibe o produto na vitrine virtual.
**Resultado esperado** | Visualizar o produto pesquisado na vitrine virtual
**Dados de entrada** | Inserção de nome de produto na caixa de pesquisa
**Prioridade**    | Média.
**Ambiente**      | Microsoft Windows 10 Pro 21H1 19043.1081, Google Chrome<br>Versão 91.0.4472.114 (Versão oficial) 64 bits.
**Técnica**       | Manual.
**Iteração**      | 1a Iteração.
 
**Caso de Teste** | **CT04 - Realizar pagamento**
 :--------------: | ------------
**Pré-Condição**  | Acessar a tela carrinho.
**Procedimento**  | 1) O ator preenche os campos solicitados no formulário<br>referente ao "Endereço de Entrega".<br>2) O ator pode selecionar a caixa checkbox "O endereço de<br>entrega é o mesmo do cadastro", que tem a função de<br>preencher o campo de endereço automaticamente, utilizando<br>os dados cadastrados, caso o ator esteja logado em sua conta.<br>3) O ator pode selecionar a caixa checkbox "Guarde essa<br>informação para a próxima vez", que tem a função de<br>preencher automaticamente os campos de endereço na<br>próxima vez que o ator preencher o formulário, caso o ator<br>esteja logado em sua conta.<br>4) O ator preenche os campos solicitados no formulário<br>"Pagamento", no qual pode escolher entre três formas de<br>pagamento.<br>5) O ator deve clicar no botão "Finalizar Compra" para finalizar<br>o pedido e enviar os formulários.<br>6) O serviço de autenticação verifica se os dados inseridos<br>são válidos, caso não sejam, o ator deve preencher novamente<br>os campos inválidos e enviar o formulário.<br>7) O sistema mostra mensagem para o ator com informação<br>do produto adquirido e data prevista de entrega.
**Resultado esperado** | Finalizar a compra de um produto
**Dados de entrada** | Dados válidos em formulários de cadastro e de pagamento
**Prioridade**    | Média.
**Ambiente**      | Microsoft Windows 10 Pro 21H1 19043.1081, Google Chrome<br>Versão 91.0.4472.114 (Versão oficial) 64 bits.
**Técnica**       | Manual.
**Iteração**      | 1a Iteração.

**Caso de Teste** | **CT05 - Visualizar Informações de Frete**
 :--------------: | ------------
**Pré-Condição**  | Acessar tela do sistema com rodapé.
**Procedimento**  | 1) O ator clica no botão "Frete" localizado no rodapé.<br>2) O sistema mostra mensagem para o ator com informações  <br>sobre o frete da loja.
**Resultado esperado** | Visualizar mensagem sobre frete da loja
**Dados de entrada** | Nenhum
**Prioridade**    | Baixa.
**Ambiente**      | Microsoft Windows 10 Pro 21H1 19043.1081, Google Chrome<br>Versão 91.0.4472.114 (Versão oficial) 64 bits.
**Técnica**       | Manual.
**Iteração**      | 1a Iteração.

## Categoria dos Testes

A categoria Teste de Funcionalidade será a técnica utilizada nos testes de software do sistema em desenvolvimento. Esta categoria tem como objetivo simular cenários de negócio - neste caso, o cenário do Sistema Web para a Loja de Roupas Bruthelu - e garantir que todos os requisitos funcionais foram implementados.


--  ----------------------------------

# Registro de Testes de Software

Na execução dos testes de software, foi possível notar as seguintes evidências:

1. *CT01 - Criar conta após preencher formulário* - Os procedimentos foram executados conforme o planejado e o resultado obtido foi parcialmente como o esperado.
2. *CT02 - Fazer Log In em conta criada* - Os procedimentos foram executados parcialmente conforme o planejado e o resultado obtido não foi como o esperado.
3. *CT03 - Procurar produto em caixa de pesquisa* - Os procedimentos foram executados parcialmente conforme o planejado e o resultado obtido não foi como o esperado.
4. *CT04 - Realizar pagamento* - Os procedimentos foram executados parcialmente conforme o planejado e o resultado obtido não foi como o esperado.
5. *CT05 - Visualizar Informações de Frete* - Os procedimentos foram executados conforme o planejado e o resultado obtido foi parcialmente como o esperado.

## Avaliação

Os resultados dos testes podem ser considerados satisfatórios, levando em conta que a parte funcional básica do sistema foi executada. Por exemplo, elementos interativos como botões, campos de preenchimento em formulários e caixas checkbox.

Nos cinco casos de teste, foi observado que as implementações efetuadas no sistema tiveram destaque, especialmente a adição de funções que permitem o sistema ficar mais interativo. Não menos importante, vale ressaltar a parte visual do sistema, que também está bem avançada, mas não se encaixa nessa categoria de teste.

As implementações acrescentadas foram positivas, porém os testes também apresentaram falhas. Duas funcionalidades testadas, *CT01* e *CT02*, nas quais se relacionam e necessitam enviar e receber dados do LocalStorage, ainda não realizam essa interação. Somente uma delas (CT01) envia e recebe dados do LocalStorage, o que compromete a interação do ator com o sistema. Outra funcionalidade, *CT03*, apresenta uma falha que envolve o LocalStorage, sendo que só é possível preencher o campo para pesquisar o produto e fazer o pedido de busca, mas não existe nenhum produto cadastrado, o que não retorna o resultado esperado. No *CT04*, os pontos positivos foram destaque, mas como se trata de validação de dados financeiros em um sistema web de um projeto acadêmico, o resultado não pôde ser como o esperado. A funcionalidade *Visualizar Informações de Frete*, pode ser considerada a mais satisfatória, apesar do resultado, devido a mensagem exibida ser apenas "frete".

Abaixo está disposto cada caso de teste efetuado, com a descrição do que foi encontrado e o print da tela no momento do teste.

> CT01 - Criar conta após preencher formulário

Como dito, os botões e campos de preenchimento estão funcionando e interagem com o serviço de validação, porém o campo nome aceita números e o campo CEP aceita letras. Para alterar isso, será preciso adicionar uma função que restringe a inserção de determinados dados. Além disso, os dados inseridos são enviados para o LocalStorage do navegador ao enviar o formulário, nos quais podem ser usados para realizar log in em cadastro criado no sistema (essa funcionalidade ainda não foi implementada). Portanto, o resultado obtido teve um impacto alto no sistema. 

Abaixo a representação da tela no momento do teste:

![Tela Cadastro - Campos nome e CEP](img/print-cadastro-falha.png)

Figura 01 - Tela Cadastro com campos nome e CEP com dados fora do padrão

![Tela Cadastro e LocalStorage](img/print-cadastro-localstorage.png)

Figura 02 - Tela Cadastro e LocalStorage com os dados armazenados

> CT02 - Fazer Log In em conta criada

Esta funcionalidade está diretamente ligada ao cadastro de usuários no sistema e como dito, ela ainda não está recebendo os dados do LocalStorage, especificamente "email" e "senha". Inclusive este último elemento deve ser implementado no formulário de cadastro. Apesar disso, os botões, campos de preenchimento e caixa checkbox funcionaram, mas o resultado não foi como esperado, gerando um impacto alto no sistema.

Abaixo a representação da tela no momento do teste:

![Tela Conta - Fazer Log In](img/print-conta-falha.png)

Figura 03 - Tela Conta opção de fazer log in

> CT03 - Procurar produto em caixa de pesquisa

A funcionalidade pesquisar produto é outra que está pendente de cadastro de dados no LocalStorage. Igualmente as outras funcionalidades, o botão para efetuar a pesquisa funcionou, porém o produto pesquisado não foi exibido na vitrine. Neste caso, o botão está programado para redirecionar o usuário para a tela de pagamento. Desse modo, o resultado obtido não foi como esperado, gerando um impacto médio no sistema.

Abaixo a representação da tela no momento do teste:

![Tela Inicial - Pesquisar produto](img/print-pesquisar-localstorage.png)

Figura 04 - Tela Inicial opção de pesquisar produto

> CT04 - Realizar pagamento

Nesta funcionalidade, as implementações visuais realizadas quanto aos campos obrigatórios foram relevantes, inclusive serão utilizadas em outros formulários. Porém, apresenta a mesma falha do formulário de cadastro, na qual os campos que deveriam aceitar apenas letras, aceitam números e campos que deveriam aceitar apenas números, aceitam letras. Foi explicado que essa funcionalidade é apenas uma simulação da venda de um produto, portanto não implica em uma venda real. Assim, no formulário "Pagamento", os dados não devem ser comparados com a realidade. Além disso, ainda não existe produto armazenado no LocalStorage, o que impossibilita a venda simulada. Portanto, o resultado obtido não foi como esperado, tendo um impacto médio no sistema.

Abaixo a representação da tela no momento do teste:

![Tela Carrinho - Pagamento](img/print-pagamento-falha.png)

Figura 05 - Tela Carrinho com campos fora do padrão

> CT05 - Visualizar Informações de Frete

O botão interativo das informações de frete da loja está funcionado corretamente, porém a mensagem exibida precisa ser reformulada. Para resolver isso basta alterar a mensagem. Assim, o resultado pode ser considerado como o esperado, gerando um impacto baixo no sistema.

Abaixo a representação da tela no momento do teste:

![Tela Inicial - Frete](img/print-frete-falha.png)

Figura 06 - Tela Inicial com mensagem "frete" exibida pelo sistema

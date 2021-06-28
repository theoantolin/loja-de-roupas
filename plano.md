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
**Procedimento**  | 1) O ator clica no botão "Frete" localizado no rodapé.<br>2) O sistema mostra mensagem para o ator com informações<br>sobre o frete da loja.
**Resultado esperado** | Visualizar mensagem sobre frete da loja
**Dados de entrada** | Nenhum
**Prioridade**    | Baixa.
**Ambiente**      | Microsoft Windows 10 Pro 21H1 19043.1081, Google Chrome<br>Versão 91.0.4472.114 (Versão oficial) 64 bits.
**Técnica**       | Manual.
**Iteração**      | 1a Iteração.


<table>
		<tr>
			<th>Tabelas de Requisitos</th>
			<th></th>
		</tr>
		<tr>
			<th>Caso de Teste</th>
			<th>CT05 - Visualizar Informações de Frete</th>
		</tr>
	<tr>
		<th>Pré-Condição</th>
		<td>
			<ol>
				<li>O ator clica no botão "Frete" localizado no rodapé.</li>
				<li>O sistema mostra mensagem para o ator com informações sobre o frete da loja.</li>
				<li>3) O ator pode selecionar a caixa checkbox "Guarde essa
informação para a próxima vez", que tem a função de
preencher automaticamente os campos de endereço na
próxima vez que o ator preencher o formulário, caso o ator
					esteja logado em sua conta.</li>
			</ol>	
		</td>
	</tr>
		<tr></tr>
		<tr></tr>
</table>

**Caso de Teste** | **CT05 - Visualizar Informações de Frete**
 :--------------: | ------------
**Pré-Condição**  | Acessar tela do sistema com rodapé.
**Procedimento**  | 1.

O ator clica no botão "Frete" localizado no rodapé.O sistema mostra mensagem para o ator com informações<br>sobre o frete da loja.
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

Nos cinco casos de teste, foi observado que as implementações efetuadas no sistema, especialmente a adição de funções que permitem o sistema ficar mais interativo, tiveram destaque. Não menos importante, vale ressaltar a parte visual do sistema, que também está bem avançada, mas não se encaixa nessa categoria de teste.

As implementações acrescentadas foram positivas, porém os testes também apresentaram falhas. Duas funcionalidades testadas que se relacionam e que necessitam enviar e receber dados para o LocalStorage, ainda não realizam essa interação, somente uma delas envia e recebe dados do LocalStorage. Outra funcionalidade apresenta uma falha que envolve o LocalStorage, sendo que só é possível preencher o campo para pesquisar o produto e fazer o pedido de busca, mas não existe nenhum produto cadastrado, o que não retorna o resultado esperado. No *CT04*, os pontos positivos tiveram realce, mas como se trata de validação de dados financeiros em um sistema web de um projeto acadêmico, o resultado não pôde ser como o esperado.






Discorra sobre os resultados do teste. Ressaltando pontos fortes e fracos identificados na solução. Comente como o grupo pretende atacar esses pontos nas próximas iterações. Apresente as falhas detectadas e as melhorias geradas a partir dos resultados obtidos nos testes.





+ No primeiro teste foi encontrado um erro. No campo é possível digitar números e no campo CEP é possível digitar letras. O impacto foi baixo.
+ No segundo teste foi possível encontrar um erro que o campo email nao está associado ao banco de dados. Ao clicar no botão entrar o usuário é direcionado para a mesma página. O impacto foi alto.
+ No terceiro teste o erro encontrado foi que não estava associado os produtos da vitrine com o campo de pesquisa. O impacto foi médio.
+ No quarto teste o erro encontrado foi que dava para digitar números no campo nome e dava para digitar letras no campo letras. O checkbox do endereço de entrega igual ao endereço de cadastro ainda não está sendo funcional. O impacto foi alto.
+ No quinto teste o erro foi que ao clicar no botão aparecia escrito apenas "frete". Para resolver esse erro basta apenas alterar a mensagem que aparecia. O impacto foi baixo.

Relatório com as evidências dos testes de software realizados no sistema pela equipe, baseado em um plano de testes pré-definido.

Descrição					Descreva    em    poucas    palavras    o    defeito encontrado.

Categoria de Teste			Indique  em  qual  categoria  foi  encontrado  o defeito.

Impacto				Baixo, Médio ou Alto?

Reprodução passo a passo			Descreva detalhadamente todos os passos até o defeito ser apresentado.

Evidência					Print da tela de erro.

Proposta de Correção				Descreva   detalhadamente   uma   proposta   de correção para o erro.

## Avaliação

Discorra sobre os resultados do teste. Ressaltando pontos fortes e fracos identificados na solução. Comente como o grupo pretende atacar esses pontos nas próximas iterações. Apresente as falhas detectadas e as melhorias geradas a partir dos resultados obtidos nos testes.

> **Links Úteis**:
> - [Ferramentas de Test para Java Script](https://geekflare.com/javascript-unit-testing/)


+ No primeiro teste foi encontrado um erro. No campo é possível digitar números e no campo CEP é possível digitar letras. O impacto foi baixo.
+ No segundo teste foi possível encontrar um erro que o campo email nao está associado ao banco de dados. Ao clicar no botão entrar o usuário é direcionado para a mesma página. O impacto foi alto.
+ No terceiro teste o erro encontrado foi que não estava associado os produtos da vitrine com o campo de pesquisa. O impacto foi médio.
+ No quarto teste o erro encontrado foi que dava para digitar números no campo nome e dava para digitar letras no campo letras. O checkbox do endereço de entrega igual ao endereço de cadastro ainda não está sendo funcional. O impacto foi alto.
+ No quinto teste o erro foi que ao clicar no botão aparecia escrito apenas "frete". Para resolver esse erro basta apenas alterar a mensagem que aparecia. O impacto foi baixo.










Usuário preenche o Nome, Nome de usuário, E-Mail, DDD, Celular, Endereço, Estado, Cidade, CEP

Bruthelo Moda Feminina

Plano de Testes Versão: 1.0

Integrantes da Equipe Bruno Theo Luiz

DESCRIÇÃO DO DOCUMENTO

OBJETIVO Plano de teste do software Bruthelo Moda Feminina LOCALIZAÇÃO GitHub

HISTÓRICO DE VERSÕES DO DOCUMENTO

VERSÃO DESCRIÇÃO DATA RESPONSÁVEL 0.1.0 Index da página principal 07/06/2021 Theo 0.1.0 Upload do arquivo Zip do Projeto 14/06/2021 Luiz 0.1.0 Atualização das páginas principais e adição dos arquivos Javascript 19/06/2021 Theo 0.2.0 Adição da página “Cadastro de usuário” 20/06/2021 Bruno 0.2.0 Layout, ajuste visual das páginas 22/07/2021 Luiz 0.2.0 Adição funcionais dos ícones e formulários, Conta, Carrinho, Favoritos 23/06/2021 Luiz 0.2.0 Teste de validação do campo número de telefone 23/06/2021 Theo 0.2.0 Ajuste e revisão de consistência dos módulos dos ícones funcionais 24/06/2021 Luiz 0.2.0 Ajuste do código das páginas: Inicial, Cadastro e Carrinho 24/06/2021 Theo

APROVAÇÕES INTERNAS

PERFIL NOME DATA Analista de Sistemas XXXX XX/XX/XXXX Analista de Qualidade XXXX XX/XX/XXXX

ÍNDICE

VISÃO GERAL 4 1.1 OBJETIVO 4 1.2 DESCRIÇÃO DO PRODUTO A SER TESTADO 4

ESCOPO 4 2.1 DESCRIÇÃO DE CASOS DE USO 4

ITENS-ALVO DOS TESTES 4

RESUMO DOS TESTES PLANEJADOS 4

CATEGORIAS DE TESTES 5 5.1 TESTE DE FUNCIONALIDADE 5 5.2 TESTE DE SEGURANÇA 5 5.3 TESTE DE USABILIDADE 5 5.4 TESTE DE PERFORMANCE 5 5.5 TESTE DE CARGA 5 5.6 TESTE DE CONFIGURAÇÃO 5 5.7 TESTE DE RECUPERAÇÃO 5 5.8 TESTE DE CONTINGÊNCIA 5

RELATÓRIO DE DEFEITOS 5

FLUXO DE TRABALHO DE TESTE 6

RECURSOS 6 8.1 HARWARE 6 8.2 SOFTWARE 6

RESPONSABILIDADES, PERFIL DA EQUIPE E NECESSIDADES DE TREINAMENTO 6 9.1 PESSOAS E PAPÉIS 6 9.2 NECESSIDADES DE TREINAMENTO 7

CRONOGRAMA E MARCOS DO PROJETO 7

VISÃO GERAL

1.1 Objetivo

O documento do Plano de Testes tem como objetivo listar os Requisitos que serão testados recomendando e descrevendo as estratégias a serem empregadas nesses testes. Este documento também identifica os recursos necessários e disponibiliza uma estimativa dos esforços de teste.

1.2 Descrição do produto a Ser Testado

Software tem como objetivo a gestão e logística de uma loja de roupas femininas em ambiente Web.

ESCOPO
2.1 Descrição de Casos de Uso

Filtro de produtos




ITENS-ALVO DOS TESTES
1 - Usuário pode criar conta no site após preencher formulário de cadastro 

2 - Usuário pode acessar conta no site utilizando login e senha 

3 - Usuário pode procurar produto pelo nome em caixa de pesquisa 

4 - Usuário pode escolher a forma de pagamento 

5 - Usuário pode clicar em texto no rodapé da página e visualizar regras de frete




RESUMO DOS TESTES PLANEJADOS
1.0 – Criar a conta do usuário 1.1 – Acessar a tela de cadastro do usuário 1.2 – Usuário preenche o Nome, Nome de usuário, E-Mail, DDD, Celular, Endereço, Estado, Cidade, CEP 1.3 – Usuário clica no botão Enviar 1.4 – Aparece a mensagem Cadastro concluído

2.0 – Acesso a conta do usuário 2.1 – Usuário preenche o e-mail 2.2 – Usuário preenche a senha 2.3 – Usuário tem a opção de clicar na opção chekbox lembre de mim 2.4 – Usuário clica no botão Entrar 2.5 – Usuário e direcionado a Pagina principal logado em sua conta

3.0 – Pesquisas por produtos na barra de navegação 3.1 – Usuário preenche a caixa de pesquisa 3.2 – Usuário clica no botão pesquisa 3.3 – O Resultado e filtrado e aparece os produtos na vitrine

4.0 – Escolher a forma de pagamento 4.1 – O usuário clica no ícone carrinho 4.2 – O usuário preenche o Endereço de Entrega, País, Estado, CEP 4.2 – O usuário clica no checkbox Cartão de crédito ou Cartão de débito ou PayPal 4.2 – O usuário preenche o Nome do cartão, Número do cartão, Vencimento, CVV 4.2 – O usuário clica no botão Continue para finalizar a compra 4.2 – Aparece a mensagem Efetuada com sucesso

5.0 – Visualizar as regras de frete 5.1 – Usuário clica no botão Frete localizado no rodapé 5.2 – Aparece uma mensagem com as informações do tipo de frete


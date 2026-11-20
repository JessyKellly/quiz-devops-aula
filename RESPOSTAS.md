# Respostas da aula guiada

Equipe: Quinha

Integrantes:
Jessy Kelly Bacelar
Gustavo Carvalho
Eduardo Fontes
Tiago Aragão
Gabriel Victor Muniz
Rafael Santos
Vitor Eduardo Assis

[Repositório](https://github.com/JessyKellly/quiz-devops-aula)

Endereço publicado

Responda Q01 a Q22 em equipe. Cada integrante deve registrar suas respostas próprias a Q23 e Q24. Registre previsões antes de executar e use a linha Observação após o resultado.

## Etapa 01 Preparação do projeto e das contas

### Q01

Se queremos automatizar os testes e disponibilizar o site por um endereço, qual responsabilidade cabe ao GitHub Actions e qual cabe ao GitHub Pages?

Resposta: O Actions automatiza as tarefas e o Pages é o serviço que hospeda a página.

Observação após a execução

### Q02

Que problema operacional pode ocorrer se cada integrante publicar uma cópia diferente do código sem registrar a versão utilizada?

Resposta: Não seria possível identificar qual seria a versão final correta pois os commits não teriam identificação de qual código base foi utilizado.

Observação após a execução

Evidência

Anote no arquivo de respostas o link do repositório e o nome da branch.

## Etapa 02 Código inicial e primeiro commit

### Q03

Que informação o commit registra para que outra pessoa consiga localizar esta entrega depois?

Resposta: O commit registra o identificador curto do commit. 


### Q04

O que pode acontecer com nosso pipeline se site/index.html ficar dentro de projeto_inicial/site/index.html no repositório?

Resposta: Ele não encontra o caminho para o arquivo.

Observação após a execução

Evidência

Copie a mensagem e o identificador curto do commit. Para consultar, use o histórico de commits da aba Code ou History em um arquivo.

## Etapa 03 Mudança identificável e histórico

### Q05

Se uma execução futura apresentar um erro, por que devemos anotar o identificador do commit associado a ela?

Resposta: Para poder voltar a versão onde a versão em questão não tinha sido publicada.

Observação após a execução

### Q06

A mudança do título já iniciou algum teste automático neste momento? O que ainda precisamos configurar?

Resposta: Não. Precisamos configurar as ações.

Observação após a execução

Evidência

Registre o identificador do novo commit e descreva em uma frase a diferença entre as duas versões.

## Etapa 04 Regra de negócio que será protegida

### Q07

Por que executar testes sobre a mesma função utilizada pela interface ajuda a verificar a versão que vamos publicar?

Resposta: Testar a função reduz a distância entre o ambiente de teste e o ambiente de produção 

Observação após a execução

### Q08

Defina o resultado esperado para três acertos e para nenhuma resposta marcada. Qual regra sustenta sua previsão?

Resposta: O resultado para 3 acertos são 3 pontos e o resultado para nenhuma resposta marcada é o retorno de 0 onde a função já prevê o nulo e o undefined  .

Observação após a execução

Evidência

Escreva no arquivo de respostas os dois resultados previstos e o caminho da função.

## Etapa 05 Testes automatizados e comando do projeto

### Q09

Qual é a sequência entre npm test, package.json e os arquivos de teste?

Resposta: Primeiro faz o arquivo de teste, depois configura o script com sua ativação no package.json e por ultimo chama o npm test

Observação após a execução

### Q10

Se o runner executar zero testes e terminar sem erro, isso é evidência suficiente para liberar a versão? O que você conferiria?

Resposta: Não. É preciso verificar se os testes foram descobertos e se foram executados corretamente, também verificar se o caminho do arquivo está correto.

Observação após a execução

Evidência

Registre os caminhos do arquivo de teste e do package.json e o comando definido para os testes.

## Etapa 06 Primeiro workflow de integração contínua

### Q11

Preveja se o commit que cria esse YAML na main inicia o pipeline. Qual evento e qual filtro do arquivo justificam sua resposta?

Resposta: Sim ele inicia o pipeline automaticamente. O evento Push e o filtro branch main.

Observação após a execução

### Q12

Qual é a vantagem de registrar o workflow no mesmo histórico do código da aplicação?

Resposta: Tratar o pipeline como parte do projeto/produto com versionamento.

Observação após a execução

Evidência

Registre o caminho do YAML e o identificador do commit que o criou.

## Etapa 07 Execução no Actions e leitura dos logs

### Q13

Por que configuramos a versão do Node.js no runner? No trecho, o que significam v7 e 24?

Resposta

Observação após a execução

### Q14

Que dados do log você registraria para comprovar que esta revisão foi verificada? Indique também a diferença entre uses e run.

Resposta

Observação após a execução

Evidência

Cole os links da execução automática e da manual e o resumo real dos testes. Identifique o evento observado em cada uma.

## Etapa 08 Falha controlada e correção

### Q15

Antes de executar, quais dos cinco casos você prevê que falharão ao dobrar o ponto por acerto? Justifique.

Resposta

Observação após a execução

### Q16

Por que reexecutar a execução defeituosa não substitui fazer o commit da correção? Use os identificadores das execuções na explicação.

Resposta

Observação após a execução

Evidência

Registre links das execuções com erro e corrigida. Copie esperado e recebido de pelo menos um teste reprovado.

## Etapa 09 Publicação condicionada e configuração do Pages

### Q17

O que needs: testes exige antes de permitir o job publicar neste workflow? Por que o nome usado é testes?

Resposta

Observação após a execução

### Q18

Como a publicação automática deste exercício caracteriza implantação contínua? Como seria uma liberação com decisão humana após os testes?

Resposta

Observação após a execução

Evidência

Registre o commit que alterou o workflow e copie a linha que conecta os jobs.

## Etapa 10 Artefato publicado e mudança visível

### Q19

O que o path ./site seleciona para o artefato de publicação? Por que precisamos conferir esse caminho?

Resposta

Observação após a execução

### Q20

Que evidências ligam a alteração do título à versão que está no endereço publicado?

Resposta

Observação após a execução

Evidência

Registre o endereço do site, o commit do novo título e o link da execução que publicou essa mudança.

## Etapa 11 Bloqueio de uma versão com defeito

### Q21

A execução com falha retirou o site do ar? Explique o que você observou no endereço publicado e no job publicar.

Resposta

Observação após a execução

### Q22

Como a mesma evidência demonstra integração contínua e controle da implantação? Identifique cada parte do processo.

Resposta

Observação após a execução

Evidência

Registre o link da execução com testes reprovados e publicar skipped e o link da recuperação com ambos aprovados.

## Etapa 12 Novo teste e explicação individual do pipeline

### Q23

Integrante

Se alguém remover needs: testes do job publicar, a falha de testes ainda garante o bloqueio? Qual configuração você restauraria e como comprovaria a correção?

Resposta

Observação após a execução

### Q24

Integrante

Escolha um comportamento de uma aplicação que seu grupo poderia construir. Proponha um teste com entrada e resultado esperado e explique em que momento do pipeline ele deve executar.

Resposta

Observação após a execução

Evidência

Registre o link da execução final com seis testes e complete as duas respostas individuais com identificação de cada integrante.

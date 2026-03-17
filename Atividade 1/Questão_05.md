# Estudo de Caso de Falha em Computação em Nuvem

Em **28 de fevereiro de 2017**, a região **US-EAST-1**, no Norte da Virgínia, da **Amazon Web Services (AWS)** sofreu uma grande interrupção que durou cerca de **4 horas**. O problema aconteceu durante uma manutenção rotineira no sistema de faturamento do **Amazon S3**, serviço de armazenamento de objetos da AWS.

Durante esse procedimento, um engenheiro executou um comando para remover alguns servidores de um subsistema do S3. Porém, um dos parâmetros foi digitado de forma incorreta, fazendo com que fossem removidos muito mais servidores do que o planejado. Esse erro acabou afetando componentes importantes do serviço.

A falha atingiu dois subsistemas críticos do S3 e gerou um efeito em cadeia, já que esse serviço serve de base para vários outros recursos da AWS. Com isso, serviços internos como o **console de gerenciamento da AWS**, o **Amazon EC2** e o **AWS Lambda** ficaram instáveis ou indisponíveis na região afetada.

O impacto também alcançou clientes externos. Diversas plataformas conhecidas, como **Netflix, Trello, Quora, IFTTT e Adobe**, apresentaram falhas totais ou parciais durante a interrupção. Um detalhe curioso foi que até mesmo o **painel de status da AWS**, que deveria informar o problema, continuou indicando situação normal por depender do próprio S3 para atualizar seus alertas.

A causa principal da falha foi a combinação de **erro humano** com a ausência de mecanismos de proteção mais rígidos nas ferramentas operacionais. Na prática, o sistema permitia a execução de comandos de grande impacto sem travas de segurança suficientes para evitar esse tipo de situação.

Para resolver o problema, a AWS precisou reiniciar os sistemas afetados, um processo que levou tempo por causa da grande quantidade de metadados que precisavam ser verificados durante a recuperação. Depois do incidente, a empresa adotou medidas preventivas, como limitar a remoção rápida de servidores abaixo de certos níveis de segurança e melhorar a separação entre subsistemas, reduzindo o risco de falhas semelhantes no futuro.

## Fonte da informação

[AWS - Resumo da interrupção do serviço Amazon S3 (em inglês)](https://aws.amazon.com/pt/message/41926/)

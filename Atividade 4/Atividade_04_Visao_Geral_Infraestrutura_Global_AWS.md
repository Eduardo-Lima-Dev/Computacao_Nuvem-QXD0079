# Atividade 04 - Visão geral da infraestrutura global da AWS

## Questão 01

Resolva o **Teste de Conhecimento do Módulo 3: Visão geral da
infraestrutura global da AWS**.

------------------------------------------------------------------------

## Questão 02

### 1. Quais os fatores que você deve considerar na seleção de uma região da AWS?

-   **Latência (proximidade):** quanto mais perto dos usuários, menor o
    tempo de resposta.
-   **Custo:** preços variam entre regiões (computação, armazenamento e
    tráfego).
-   **Serviços disponíveis:** nem todos os serviços AWS estão
    disponíveis em todas as regiões.
-   **Conformidade e leis:** algumas aplicações exigem que os dados
    permaneçam em um país específico.
-   **Alta disponibilidade:** regiões com mais Zonas de Disponibilidade
    (AZs) permitem arquiteturas mais resilientes.

### 2. Regiões da AWS com três ou mais Zonas de Disponibilidade

-   US East (N. Virginia) -- 6 AZs
-   US East (Ohio) -- 3 AZs
-   US West (Oregon) -- 4 AZs
-   US West (N. California) -- 3 AZs
-   Africa (Cape Town) -- 3 AZs
-   Asia Pacific (Mumbai) -- 3 AZs
-   Asia Pacific (Seoul) -- 4 AZs
-   Asia Pacific (Tokyo) -- 4 AZs
-   Asia Pacific (Sydney) -- 3 AZs
-   Asia Pacific (Singapore) -- 3 AZs
-   Asia Pacific (Jakarta) -- 3 AZs
-   Asia Pacific (Osaka) -- 3 AZs
-   Canada (Central) -- 3 AZs
-   Europe (Frankfurt) -- 3 AZs
-   Europe (Ireland) -- 3 AZs
-   Europe (London) -- 3 AZs
-   Europe (Paris) -- 3 AZs
-   Europe (Stockholm) -- 3 AZs
-   Middle East (Bahrain) -- 3 AZs
-   South America (São Paulo) -- 3 AZs

------------------------------------------------------------------------

## Questão 03

### 1. Armazenamento

-   **S3** --- Armazena arquivos (objetos) de forma escalável na nuvem.
-   **EBS** --- Fornece discos virtuais para instâncias EC2.
-   **EFS** --- Sistema de arquivos compartilhado e escalável.

### 2. Computação

-   **EC2** --- Máquinas virtuais sob demanda na nuvem.
-   **Lambda** --- Executa código sem gerenciar servidores.
-   **ECS** --- Orquestra containers Docker na AWS.

### 3. Banco de Dados

-   **RDS** --- Banco relacional gerenciado.
-   **DynamoDB** --- Banco NoSQL rápido e totalmente gerenciado.
-   **Aurora** --- Banco relacional compatível com MySQL/PostgreSQL.

### 4. Rede e Entrega de Conteúdo

-   **VPC** --- Cria redes virtuais privadas.
-   **CloudFront** --- CDN com baixa latência.
-   **Route 53** --- Serviço de DNS altamente disponível.

------------------------------------------------------------------------

## Questão 04 --- Laboratório

### 1. Console AWS

-   Categoria do IAM
-   Categoria do RDS
-   Categoria do AWS Cost Explorer
-   Categoria do CloudWatch
-   Categoria do VPC

### 2. Serviço VPC

-   Alterar a região (ex.: EU London).
-   Descrever o que acontece ao trocar de região.

### 3. Sub-redes

-   Verificar zona de disponibilidade.
-   Listar a AZ de cada sub-rede.

### 4. VPCs

-   Quantidade de VPCs.
-   Identificar se a informação é por região ou por AZ.

### 5. EC2

-   Quantidade de instâncias.
-   Região de cada instância.
-   Tipo da instância e características.
-   Sistema operacional.

### 6. Página inicial da AWS

-   Listar os serviços visitados.
-   Verificar o painel **Custo e Uso**.

# ERP Logístico

## 1. Conceito

O ERP Logístico é um sistema de gestão empresarial **voltado para empresas de varejo**, com foco na organização e integração dos processos logísticos. A proposta é centralizar informações relacionadas a produtos, fornecedores, estoque, centros de distribuição, pedidos, expedição, transporte e entregas em uma única plataforma.

O sistema acompanha o fluxo operacional desde a entrada e armazenamento dos produtos até o processamento de pedidos e sua entrega ao cliente. Além do controle das operações, o sistema busca fornecer informações e indicadores que permitam acompanhar o desempenho logístico, identificar problemas e auxiliar na tomada de decisões.

## 2. Objetivos

### 2.1 Objetivo geral

Desenvolver um sistema integrado de gestão logística capaz de centralizar e controlar os principais processos relacionados à movimentação e distribuição de produtos em empresas de varejo.

### 2.2 Objetivos específicos

- Centralizar informações de produtos, fornecedores e estoques.
- Controlar estoques em diferentes centros de distribuição.
- Registrar entradas, saídas e transferências de produtos.
- Gerenciar pedidos e seus respectivos itens.
- Controlar o processo de separação e expedição.
- Gerenciar transportadoras e processos de entrega.
- Acompanhar o status dos pedidos durante o processo logístico.
- Registrar devoluções e ocorrências relacionadas às entregas.
- Disponibilizar indicadores para acompanhamento da operação logística.

## 3. Escopo

O sistema terá como foco os processos relacionados à **gestão logística do varejo**, contemplando principalmente estoque, armazenagem, pedidos, expedição, transporte e entrega.

O projeto não tem como objetivo implementar um ERP empresarial completo com todos os processos administrativos, contábeis e financeiros de uma organização. Esses processos podem ser considerados externos ao escopo ou representados de forma simplificada quando forem necessários para os fluxos logísticos.

## 4. Módulos do Sistema

### 4.1 Gestão de Produtos

Responsável pelo cadastro e gerenciamento dos produtos comercializados pela empresa.

Principais informações:

- Nome e descrição do produto.
- Categoria.
- Código de identificação.
- Unidade de medida.
- Estoque mínimo.
- Status do produto.

### 4.2 Gestão de Fornecedores

Responsável pelo cadastro das empresas responsáveis pelo fornecimento dos produtos.

O módulo deverá permitir o registro de informações dos fornecedores e seu relacionamento com os produtos fornecidos.

### 4.3 Gestão de Estoque

Responsável pelo controle das quantidades e movimentações dos produtos armazenados.

O estoque poderá representar diferentes situações:

- Estoque disponível.
- Estoque reservado.
- Estoque em trânsito.
- Estoque indisponível.
- Estoque mínimo.

As principais operações serão:

- Entrada de produtos.
- Saída de produtos.
- Reserva de estoque.
- Liberação de reserva.
- Transferência entre centros de distribuição.
- Ajuste de inventário.

### 4.4 Centros de Distribuição

O sistema deverá permitir o gerenciamento de múltiplos centros de distribuição (CDs).

Cada centro de distribuição possuirá seu próprio estoque e poderá participar de operações como:

- Recebimento de produtos.
- Armazenamento.
- Separação de pedidos.
- Expedição.
- Transferência de produtos para outros CDs.

A existência de múltiplos CDs permite que o sistema considere a disponibilidade de estoque e a localização dos produtos durante o processamento dos pedidos.

### 4.5 Gestão de Pedidos

Responsável pelo processamento e acompanhamento dos pedidos.

Um pedido será composto por um ou mais produtos e deverá possuir informações como:

- Identificação do pedido.
- Data de criação.
- Itens.
- Quantidades.
- Centro de distribuição responsável.
- Status.
- Informações de entrega.

O sistema deverá verificar a disponibilidade dos produtos antes que o pedido avance para as etapas seguintes.

### 4.6 Expedição

Responsável pelas etapas posteriores à confirmação do pedido e anteriores ao transporte.

O processo envolve:

1. Separação dos produtos.
2. Conferência.
3. Embalagem.
4. Preparação para envio.
5. Expedição.

A expedição deverá estar vinculada ao pedido e ao centro de distribuição responsável.

### 4.7 Transportadoras

Responsável pelo gerenciamento das empresas responsáveis pelo transporte dos pedidos.

Podem ser armazenadas informações como:

- Nome da transportadora.
- Regiões atendidas.
- Prazo médio de entrega.
- Custo de transporte.
- Capacidade operacional.
- Status.

Essas informações poderão posteriormente ser utilizadas para auxiliar na escolha da transportadora mais adequada para cada pedido.

### 4.8 Entregas

Responsável pelo acompanhamento dos pedidos após sua expedição.

O sistema deverá registrar diferentes estados da entrega, como:

- Aguardando envio.
- Em trânsito.
- Em rota de entrega.
- Entregue.
- Atrasada.
- Devolvida.

Também poderão ser registradas ocorrências relacionadas à entrega.

### 4.9 Devoluções

Responsável pelo registro e acompanhamento de produtos devolvidos.

Uma devolução deverá estar relacionada a um pedido e poderá conter informações como:

- Motivo da devolução.
- Produtos devolvidos.
- Quantidades.
- Data.
- Status.
- Destino dos produtos após a devolução.

Quando aplicável, os produtos devolvidos poderão retornar ao estoque após avaliação.

### 4.10 Relatórios e Indicadores

O sistema deverá disponibilizar informações para acompanhamento do desempenho da operação logística.

Entre os indicadores previstos estão:

- Pedidos processados.
- Pedidos em trânsito.
- Pedidos atrasados.
- Taxa de entregas no prazo.
- Tempo médio de entrega.
- Custo médio de transporte.
- Produtos abaixo do estoque mínimo.
- Giro de estoque.
- Produtos com baixa movimentação.

## 5. Fluxo Logístico

O fluxo principal do sistema representa o caminho percorrido por um pedido desde sua criação até a entrega.

```text
Pedido
  ↓
Verificação de estoque
  ↓
Reserva de estoque
  ↓
Separação
  ↓
Conferência
  ↓
Embalagem
  ↓
Expedição
  ↓
Transportadora
  ↓
Em trânsito
  ↓
Entrega
  ↓
Pedido concluído
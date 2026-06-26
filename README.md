# Da Infraestrutura Tradicional à Computação em Nuvem: Impactos na Eficiência, Custos e Agilidade Empresarial

Análise estratégica e proposta de redesenho de processos de negócio para migração de infraestruturas legadas para o paradigma de computação em nuvem, alinhando eficiência operacional, governança e previsibilidade financeira.

---

## 📌 Sobre o Projeto

Este repositório contém o estudo de caso e o mapeamento de processos desenvolvidos para a disciplina de **Gestão de Processos de Negócios (GPN)** na **Universidade Estadual do Ceará (UECE) - Campus Avançado de Mombaça**.

O objetivo principal é analisar as transformações impostas pela computação em nuvem ao mercado de tecnologia, estabelecendo um comparativo prático entre o modelo tradicional (CAPEX) e o modelo em nuvem (OPEX), identificando os impactos multidimensionais dessa transição no ambiente corporativo.

---

## ⚙️ Descrição do Processo & Atores

O ciclo de migração fundamenta-se na modernização de sistemas legados, iniciando-se com o diagnóstico da infraestrutura vigente, avaliação de viabilidade financeira e definição do modelo de implantação (nuvem pública, privada, híbrida ou multicloud). O fluxo envolve uma equipe multidisciplinar:
*   **Gestores de TI:** Responsáveis pelo planejamento estratégico e aprovação de planos.
*   **Equipe de Infraestrutura & Desenvolvedores:** Executam a adequação de aplicações, migração e testes.
*   **Fornecedor do Serviço:** Responsável pela disponibilização de recursos e suporte via SLA.
*   **Usuário Final:** Fornece o feedback após o acesso e uso dos serviços migrados.

---

## ⚠️ Desafios e Problemas Identificados (As-Is)

Durante o mapeamento do fluxo linear tradicional, foram detectados os seguintes gargalos severos:
*   **Gargalos de Refatoração no Legado:** Migrar arquiteturas monolíticas sem adaptação prévia gera ciclos intermináveis de falha e retrabalho.
*   **Estouro de Orçamento (75%):** Alto índice de organizações excedem o planejamento financeiro inicial durante a migração (dados McKinsey/BCG).
*   **Risco de Downtime Prolongado:** Média histórica de até 72 horas anuais de inatividade antes da otimização.
*   **Silos de Conhecimento Operacional (41%):** Cerca de 41% da força técnica carece de proficiência imediata nas novas ferramentas, gerando dependência excessiva do fornecedor (dados Gartner).
*   **Vulnerabilidades de Conformidade:** Movimentação de grandes volumes de dados sem auditoria contínua expõe a empresa a quebras de regras de negócio.
*   **Desconexão com o Usuário:** Coletar o feedback apenas no extremo fim do fluxo pode forçar o retorno do processo à estaca zero.

---

## 🚀 Propostas de Melhoria & Redesenho (To-Be)

Para mitigar os riscos operacionais e financeiros, o processo foi otimizado com las seguintes implementações:

1.  **Infraestrutura como Código (IaC):** Automação do provisionamento via scripts (*Terraform/Ansible*) para eliminar erros e intervenções manuais do fornecedor.
2.  **Triagem de Migração (Gateway de Decisão):** Inserção de um gateway estratégico para avaliar previamente o uso de *Rehost* (Lift-and-Shift) ou *Refactor* (reconstrução nativa).
3.  **Integração de FinOps & DevSecOps:** Inclusão do rastreamento em tempo real de OPEX e auditorias de segurança durante a transferência de dados.
4.  **Centro de Excelência em Nuvem (CCoE):** Comitê multidisciplinar encarregado da governança técnica, financeira e de conformidade normativa.

### 📉 Impacto Mensurável da Otimização
*   **Eficiência Operacional:** Elevada para **94%**.
*   **Redução de Custos (OPEX):** Queda do custo anual médio de \$450.000 para **\$220.000**.
*   **Minimização de Downtime:** Reduzido de 72 horas para apenas **1 hora anual**.
*   **Mitigação de Desperdício:** Controle do desperdício de nuvem ativa (média de 32% no mercado).

---

## 📊 Dashboard Interativo de Business Intelligence

Os indicadores macroeconômicos globais, a evolução temporal e os riscos de transição foram consolidados em um dashboard interativo para validação do redesenho do fluxo.

🔗 **[Acesse o Dashboard Online no Power BI Service](https://app.powerbi.com/links/dfWMWYukbS?ctid=908c7dda-c74d-40de-947a-c8dd7f70524e&pbi_source=linkShare)**

---

## 🛠️ Como Executar e Atualizar o Arquivo PBIX Localmente

Caso você baixe o arquivo `.pbix` e ele apresente erro ao carregar os gráficos (comum quando o caminho do arquivo local muda), siga as etapas abaixo para restabelecer a conexão com a base de dados:

### 1. Vincular a Base de Dados (`.xlsx`)
O projeto utiliza como fonte de dados o arquivo **`dados_power_bi_cloud_paises_fix(1).xlsx`**. Para corrigir erros de caminho:
1. Abra o projeto no **Power BI Desktop**.
2. Na aba **Página Inicial**, clique na seta abaixo do botão **Transformar Dados** e selecione **Configurações da Fonte de Dados**.
3. Selecione o arquivo Excel listado na lista de fontes e clique em **Alterar Fonte...**.
4. Clique em **Procurar**, navegue pelas pastas do seu computador até encontrar onde salvou o arquivo `dados_power_bi_cloud_paises_fix(1).xlsx` e selecione-o.
5. Clique em **OK** e depois em **Fechar**.

### 2. Aplicar Alterações e Atualizar os Gráficos
1. Um aviso amarelo surgirá no topo da tela. Clique em **Aplicar Alterações** (ou *Apply Changes*).
2. Para garantir que toda a base de países e faturamentos foi processada com sucesso, clique no botão **Atualizar** (ou *Refresh*) localizado no menu superior da aba *Página Inicial*.
3. O Power BI reprocessará os relacionamentos e os visuais do panorama macroeconômico serão renderizados normalmente.

### 3. Publicar Atualizações (Opcional)
Caso queira atualizar os dados ou o layout e sincronizar com a versão web:
1. Clique em **Publicar** no canto superior direito do Power BI Desktop.
2. Selecione o seu Workspace de destino.
3. Substitua o relatório existente para que as modificações reflitam no link público compartilhado.

---

## 🛠️ Tecnologias & Conceitos Chave

*   **Cloud Providers:** AWS, Microsoft Azure, Google Cloud, Alibaba Cloud, Tencent Cloud.
*   **Gestão Financeira:** CAPEX vs. OPEX / FinOps (Rastreamento em tempo real).
*   **Automação & Engenharia:** IaC (Infrastructure as Code) com Terraform/Ansible.
*   **Modelagem de Processos:** BPMN (Mapeamento As-Is e To-Be).

---

## 👥 Autor

*   **Antônio Marcos Welinton Teixeira da Silva** - [antonio.welinton@aluno.uece.br](mailto:antonio.welinton@aluno.uece.br)
*   *Estudante de Sistemas de Informação - UECE Mombaça*

# Micael Levergger

Estudante de Engenharia de Software na Universidade Católica de Brasília (6º semestre, conclusão em 2027) e estagiário de tecnologia na BBTS (BB Tecnologia e Serviços) há mais de um ano. Trabalho com automação de processos, low-code, dados e integrações entre sistemas.

[Site em produção](https://alinevieiranails.com.br) · [LinkedIn](https://linkedin.com/in/micael-levergger-7906102bb) · [E-mail](mailto:micael.vasconcelos@a.ucb.br)

---

## Projeto em destaque

### Aline Vieira Nails — sistema de agendamento online

**Site:** [alinevieiranails.com.br](https://alinevieiranails.com.br)

Sistema completo de agendamento desenvolvido para uma manicure profissional, publicado com domínio próprio e em uso real por ela e suas clientes.

> ⚠️ O site atende clientes reais. Por favor, não faça agendamentos de teste.

**Funcionalidades**

- **Site público:** a cliente escolhe o serviço, a data e um horário disponível, e confirma o agendamento pelo WhatsApp.
- **Painel administrativo (acesso restrito):** agenda com cancelamento, bloqueio de dias e horários e indicadores financeiros (faturamento, comparação entre períodos, serviços e clientes mais frequentes).

**Decisões técnicas**

- **Preço validado no servidor:** um trigger no PostgreSQL substitui o nome e o valor do serviço enviados pelo navegador pelos valores cadastrados, impedindo adulteração de preço.
- **Sem agendamento duplicado:** índice único parcial em (data, horário) para agendamentos confirmados garante consistência mesmo com requisições simultâneas.
- **Permissões mínimas:** usuários anônimos só podem inserir colunas específicas (grants por coluna).
- **Dados pessoais protegidos:** funções administrativas (security definer) verificam o papel de administrador no JWT antes de retornar dados de clientes.
- **Segurança testada na prática:** chamadas reais à API simulando falsificação de preço, agendamento duplicado e acesso não autenticado às funções administrativas.

**Tecnologias:** HTML, CSS, JavaScript, Supabase (PostgreSQL, Auth, PostgREST), Netlify, domínio próprio.

*Código em repositório privado, por se tratar de um sistema de cliente.*

---

## Experiência profissional — BBTS

**Estagiário de Tecnologia** · desde jun/2025 · Brasília, DF

- Desenvolvi um sistema de marcação de ausências em Power Apps + SharePoint, com fluxos de notificação no Power Automate.
- Integrei o SharePoint à API SOAP da LG Suíte Gen.te para o agendamento de férias.
- Construí automação RPA com Power Automate Desktop para coleta de dados em portal de preços.
- Crio e mantenho subprocessos da Central de Serviços no BPMS Supravizio.
- Desenvolvo notebooks em Databricks (Python e SQL) e dashboards em Power BI.
- Realizo testes funcionais e documento os processos e fluxos implementados, em equipe com metodologias ágeis.

*Projetos corporativos: código não público.*

---

## Stack

| Área | Ferramentas |
|---|---|
| Automação e low-code | Power Automate (Cloud e Desktop/RPA), Power Apps, SharePoint, Supravizio (BPMS) |
| Dados e BI | Power BI (DAX, Power Query/M, modelagem dimensional), Python/Pandas, Databricks/Unity Catalog |
| Banco de dados | SQL, PostgreSQL, Supabase |
| Desenvolvimento web | HTML, CSS, JavaScript |
| Integrações e DevOps | APIs REST e SOAP, Git, Azure DevOps |
| Práticas | Testes funcionais, documentação de processos, metodologias ágeis |

---

## Em desenvolvimento

**Loja virtual de roupas (MVP)** — e-commerce para uma loja real de pequeno porte, com perfis de cliente e administrador, produtos com variações de tamanho e cor, categorias e pagamento via Mercado Pago (sandbox). Tecnologias: TypeScript, Next.js e PostgreSQL (Supabase).

---

## Outros projetos

| Projeto | Descrição | Tecnologias |
|---|---|---|
| [Dashboard do Cliente](https://github.com/micaellevergger213/dados) | Protótipo de painel bancário com saldos, extrato, contratação de serviços e simulação de PIX/transferência | HTML, CSS |
| [Formulário de Triagem](https://github.com/micaellevergger213/formulario) | Formulário de triagem clínica com classificação de risco por cores (Protocolo de Manchester) | HTML, CSS, Bootstrap |

---

## Contato

- **E-mail:** micael.vasconcelos@a.ucb.br
- **LinkedIn:** [linkedin.com/in/micael-levergger-7906102bb](https://linkedin.com/in/micael-levergger-7906102bb)

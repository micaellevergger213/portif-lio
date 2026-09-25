# Micael Levergger — Portfólio

Estudante de Engenharia de Software (UCB, 6º semestre, conclusão em 2027) e estagiário de tecnologia na BBTS há mais de um ano, atuando com automação, low-code, dados e integrações.

## Stack
- **Automação & Low-code:** Power Automate (Cloud e Desktop/RPA), Power Apps, SharePoint, Supravizio (BPMS)
- **Banco de dados:** SQL, PostgreSQL, Supabase
- **Desenvolvimento Web:** HTML, CSS, JavaScript
- **Dados & BI:** Power BI (DAX, Power Query/M, modelagem dimensional), Python/Pandas, Databricks/Unity Catalog
- **Integrações & DevOps:** APIs REST e SOAP, Git, Azure DevOps
- **Práticas:** testes funcionais, documentação de processos, metodologias ágeis

## Experiência profissional — BBTS
- Sistema de marcação de ausências em Power Apps + SharePoint, com fluxos de notificação no Power Automate
- Integração SharePoint → API SOAP (LG Suíte Gen.te) para agendamento de férias
- Automação RPA com Power Automate Desktop para coleta de dados em portal de preços
- Criação e manutenção de subprocessos da Central de Serviços no BPMS Supravizio
- Testes funcionais das automações e subprocessos desenvolvidos
- Documentação dos processos e fluxos implementados
- Trabalho em equipe com metodologias ágeis

> Projetos corporativos: código não público.

## Projeto em destaque

### Sistema de Agendamento para Manicure — [site em produção](https://famous-yeot-5e085d.netlify.app)
Sistema desenvolvido para uma profissional de manicure e em uso real por ela e suas clientes.

> ⚠️ Site em uso por cliente real — por favor, não realize agendamentos de teste.

**Funcionalidades**
- **Site público:** a cliente escolhe o serviço, uma data e um horário disponível, e confirma o agendamento pelo WhatsApp
- **Painel administrativo (acesso restrito):** agenda com cancelamento, bloqueio de dias e horários e indicadores financeiros (faturamento, comparação entre períodos, serviços e clientes mais frequentes)

**Decisões técnicas**
- **Preço validado no servidor:** um trigger no PostgreSQL substitui o nome e o valor do serviço enviados pelo navegador pelos valores cadastrados, impedindo adulteração de preço
- **Sem agendamento duplicado:** índice único parcial em (data, horário) para agendamentos confirmados garante consistência mesmo com requisições simultâneas
- **Permissões mínimas:** usuários anônimos só podem inserir colunas específicas (grants por coluna)
- **Dados pessoais protegidos:** funções administrativas (security definer) verificam o papel de administrador no JWT antes de retornar dados de clientes
- **Segurança testada na prática:** chamadas reais à API simulando falsificação de preço, agendamento duplicado e acesso não autenticado às funções administrativas

**Tecnologias:** HTML, CSS, JavaScript, Supabase (PostgreSQL, Auth, PostgREST), Netlify

> Código em repositório privado.

## Outros projetos
| Projeto | Descrição | Tecnologias |
|---|---|---|
| [Dashboard do Cliente](https://github.com/micaellevergger213/dados) | Protótipo de painel bancário com saldos, extrato, contratação de serviços e simulação de PIX/transferência | HTML, CSS |
| [Formulário de Triagem](https://github.com/micaellevergger213/formulario) | Formulário de triagem clínica com classificação de risco por cores (Protocolo de Manchester) | HTML, CSS, Bootstrap |

## Contato
- E-mail: micael.vasconcelos@a.ucb.br
- LinkedIn: _(adicionar)_

# RentControl

> 🇧🇷 [Português](#português) | 🇺🇸 [English](#english)

<p align="center">
  <img src="assets/img/dashboard-mockup.png" alt="RentControl dashboard no desktop e no celular" width="90%">
</p>

---

<a name="português"></a>

## 🇧🇷 Português

> Sistema de gestão de locação de imóveis: do contrato à fatura, tudo no mesmo lugar.

### O que é

RentControl é um sistema web para quem administra o aluguel de imóveis: desde famílias com algumas casas até imobiliárias pequenas com uma carteira de contratos.

A ideia central é simples: tirar do papel e das planilhas o controle de proprietários, inquilinos, contratos e pagamentos, e deixar o sistema cuidar do que é repetitivo, como gerar faturas todo mês e cobrar multa por atraso automaticamente.

### Origem

O RentControl nasceu como ideia de TCC e foi sendo moldado ao longo do desenvolvimento até se tornar um projeto com ambição real: um sistema por assinatura (SaaS) voltado para quem administra imóveis no dia a dia. O que começou como trabalho acadêmico está virando um produto em construção.

### O problema que resolve

Quem aluga imóveis hoje costuma depender de planilhas espalhadas: uma para os contratos, outra para os pagamentos, um caderno para lembrar quem está atrasado. Esse modelo funciona até o dia em que não funciona: um aluguel que ninguém cobrou, um contrato vencido que passou despercebido, uma multa calculada errada.

O RentControl centraliza esse controle em um único sistema. Cada imóvel sabe se está disponível ou alugado. Cada contrato sabe quando vence e qual é o índice de reajuste. O sistema gera as faturas do mês sozinho e aplica encargos em caso de atraso, sem depender de ninguém lembrar de fazer isso na mão.

### Funcionalidades disponíveis

**Faturamento automático**
Todo mês o sistema gera as faturas de cada contrato ativo (aluguel + condomínio + IPTU) e confere a inadimplência todos os dias, sem nenhuma intervenção manual.

**Multa e juros automáticos**
Multa de 2% e juros de 1% ao mês, pro rata die, aplicados automaticamente sobre o valor em atraso assim que o vencimento passa.

**Contratos completos**
Ligam imóvel e inquilino com vencimento, tipo de garantia (caução, fiador ou seguro-fiança) e reajuste anual automático por IGPM ou IPCA. O imóvel some da lista disponível ao alugar e volta ao encerrar o contrato.

**Cadastro rápido com consulta de CNPJ**
A consulta à Receita Federal preenche os dados do proprietário automaticamente a partir do CNPJ, sem digitação manual.

**Relatório de rentabilidade**
Receita realizada, yield anual e taxa de ocupação por período, imóvel a imóvel, para saber exatamente quanto cada propriedade está rendendo.

**Notificações automáticas por e-mail**
O sistema envia dois tipos de e-mail sem nenhuma ação manual:

- **Para o inquilino:** assim que a fatura é gerada, ele recebe o descritivo completo (aluguel, condomínio, IPTU, total e vencimento) junto com a chave Pix do proprietário e os dados bancários para pagamento.
- **Para o proprietário:** um resumo mensal com todas as faturas dos seus imóveis, o total recebido e os valores em aberto, imóvel a imóvel.

**Repasse organizado e acesso seguro**
Chave Pix e dados bancários do proprietário guardados para o repasse, com autenticação JWT e perfis de administrador ou operador.

### Em breve

**Pagamento dentro do sistema**
Hoje o inquilino paga via Pix usando a chave enviada por e-mail. O próximo passo é o inquilino poder escolher entre Pix, boleto ou cartão diretamente no sistema, com a fatura conciliada automaticamente ao confirmar o pagamento.

**Portal do inquilino**
Login próprio para o inquilino acompanhar o status da fatura do mês, ver o histórico de pagamentos, baixar comprovantes e consultar os dados do contrato, sem precisar ligar para o gestor.

**Rentabilidade com todos os gastos**
Registro de manutenções e outras despesas de cada imóvel para calcular a rentabilidade real do patrimônio, não só o aluguel recebido.

### Como o sistema funciona

```
1. Cadastre proprietários, imóveis e inquilinos em segundos, com consulta automática de CNPJ
2. Ligue imóvel e inquilino: defina vencimento, garantia e reajuste
3. O sistema gera as faturas todo mês e avisa sozinho quem atrasou
```

---

<a name="english"></a>

## 🇺🇸 English

> Property rental management system: from contract to invoice, everything in one place.

### What it is

RentControl is a web system for anyone who manages rental properties: from families with a few homes to small real estate agencies with a full portfolio of contracts.

The core idea is simple: move the control of owners, tenants, contracts, and payments out of spreadsheets and let the system handle the repetitive work, like generating invoices every month and automatically charging late fees.

### Origin

RentControl started as a college thesis idea and was shaped throughout development into a project with real ambition: a subscription-based system (SaaS) for people who manage rental properties day to day. What began as academic work is becoming a product in progress.

### The problem it solves

Most landlords today rely on scattered spreadsheets: one for contracts, one for payments, a notebook to remember who's overdue. That setup works until it doesn't: a missed invoice, an expired contract no one noticed, a late fee calculated wrong.

RentControl centralizes all of that in a single system. Each property knows whether it is available or rented. Each contract knows when it expires and what the adjustment index is. The system generates monthly invoices on its own and applies late charges automatically, with no one needing to remember to do it manually.

### Available features

**Automatic billing**
Every month the system generates invoices for each active contract (rent + condo fee + property tax) and checks for overdue payments daily, with no manual action required.

**Automatic late fees**
A 2% fine plus 1% monthly interest, pro rata die, applied automatically to the overdue amount as soon as the due date passes.

**Complete contracts**
Contracts link a property and a tenant, setting the due date, guarantee type (deposit, guarantor, or surety insurance), and automatic annual adjustment by IGPM or IPCA. The property is removed from the available list when rented and returns when the contract ends.

**Fast registration with CNPJ lookup**
An automatic query to the Brazilian Federal Revenue fills in the owner's details from the CNPJ, with no manual typing.

**Profitability report**
Realized revenue, annual yield, and occupancy rate by period, property by property, so you know exactly how much each one is returning.

**Automatic email notifications**
The system sends two types of emails with no manual action:

- **To the tenant:** as soon as the invoice is generated, they receive the full breakdown (rent, condo fee, property tax, total, and due date) along with the owner's Pix key and banking details for payment.
- **To the owner:** a monthly summary with all invoices for their properties, total received, and amounts outstanding, property by property.

**Organized transfers and secure access**
Owner's Pix key and banking details stored for rent transfers, with JWT authentication and administrator or operator user profiles.

### Coming soon

**In-system payment**
Today tenants pay via Pix using the key sent by email. The next step is letting them choose between Pix, bank slip (boleto), or card directly in the system, with the invoice automatically reconciled upon payment confirmation.

**Tenant portal**
A dedicated login for tenants to track their monthly invoice status, view payment history, download receipts, and check contract details without needing to call the manager.

**Full profitability with all expenses**
Register maintenance and other costs per property to calculate the real return on the asset, not just the rent received.

### How it works

```
1. Register owners, properties, and tenants in seconds with automatic CNPJ lookup
2. Link property and tenant: set due date, guarantee type, and adjustment index
3. The system generates invoices every month and automatically flags who is late
```

---

## Licença / License

Este repositório é privado. Todos os direitos reservados.
This repository is private. All rights reserved.

---

Desenvolvido por / Developed by [Antônio Marcos Goulart](https://github.com/Antonio-Marcos-Goulart)

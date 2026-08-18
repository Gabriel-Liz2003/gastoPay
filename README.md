# GastoPay

Aplicativo Android pessoal para acompanhar gastos feitos via Google Wallet/Google Pay e usar notificações do Nubank como backup.

## Objetivo

Ao detectar uma compra, o app registra o valor localmente, atualiza quanto ainda pode ser gasto no ciclo e pode criar um evento temporário no Google Agenda para a automação do ChatGPT processar.

## Privacidade

- O app filtra notificações do Google Wallet e Nubank.
- Não envia número do cartão.
- Não salva o texto bruto das notificações na ponte.
- O histórico financeiro principal fica no aparelho.
- O app não declara permissão INTERNET; a ponte usa o provedor de Agenda do Android.

## Como instalar pelo celular

1. Abra a aba **Actions** deste repositório.
2. Abra a execução mais recente de **Build Android APK**.
3. Em **Artifacts**, baixe `GastoPay-debug-apk`.
4. Extraia o ZIP baixado.
5. Instale `app-debug.apk` no Android.
6. Abra o GastoPay e libere acesso às notificações.
7. Libere acesso ao Google Agenda quando solicitado.

## Build

O GitHub Actions extrai `GastoPay.zip`, executa os testes unitários e gera o APK debug automaticamente.

## Orçamento inicial

A versão atual começa com orçamento de R$ 470,00, que pode ser alterado dentro do app.

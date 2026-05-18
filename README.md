# Observer v1.0.14 — Manual do Usuário

Este guia é para o usuário final e explica como configurar e usar o Observer no dia a dia.

---

## 1. Visão geral

O Observer é um aplicativo que monitora uma pasta de XMLs fiscais e envia os arquivos automaticamente para a plataforma Embed. Ele foi feito para rodar silenciosamente em segundo plano, com acesso rápido pela bandeja do sistema.

---

## 2. Primeiro acesso (Setup)

Ao abrir o aplicativo pela primeira vez, você passará por algumas telas de configuração. Elas são simples e guiadas.

### 2.1. Tela “RESPONSÁVEL PELA INTEGRAÇÃO”

Nesta tela, você informa o **CNPJ da Responsável pela Integração** responsável pelo seu sistema.

- Se você **não tiver** o CNPJ, basta clicar em **SALVAR** para usar o padrão Embed.
- Se informar um CNPJ, o Observer valida automaticamente.

Ações disponíveis:
- **SALVAR**: valida o CNPJ e avança.
- **SAIR**: fecha o aplicativo.

### 2.2. Tela de confirmação do Responsável pela Integração

Aparece uma mensagem de sucesso após a validação.
- Clique em **PRÓXIMO** para continuar.

### 2.3. Tela “ESTABELECIMENTO COMERCIAL”

Aqui você informa os dados do estabelecimento:

- **CNPJ**
- **E-mail**
- **Telefone**
- **Loja (opcional)**: se quiser, informe um apelido do caixa/PDV, ex: “Caixa 01”.

O sistema também identifica automaticamente o **PDV ID** (geralmente o MAC Address da máquina).

Ações disponíveis:
- **SALVAR**: envia os dados e registra o PDV.
- **SAIR**: fecha o aplicativo.

### 2.4. Tela “CONFIRMAÇÃO”

Após o cadastro, um **código de 4 dígitos** é enviado por e-mail. Digite o código e clique em **SALVAR**.

Ações disponíveis:
- **SALVAR**: confirma o PDV.
- **SAIR**: fecha o aplicativo.

### 2.5. Tela de sucesso

Quando o PDV está ativo, você verá “Terminal ativado com sucesso!”.
Clique em **PRÓXIMO** para configurar o monitoramento.

### 2.6. Tela “MONITORAMENTO”

Nesta tela você seleciona a pasta onde os XMLs ficam salvos.

- Clique em **BUSCAR** e escolha a pasta correta.
- Clique em **SALVAR** para iniciar o monitoramento.

### 2.7. Tela “MONITORAMENTO ATIVADO”

Confirma que o monitoramento foi iniciado.
Clique em **INICIAR** para ir para a tela principal do app.

---

## 3. Tela principal (Status)

Após o setup, o Observer exibe a tela de status com informações do processamento.

Mensagens comuns:
- **“Aguardando arquivo para processamento”**
- **“Arquivo X sendo processado”**

O app continua rodando mesmo quando você fecha a janela, ficando disponível na bandeja do sistema.

---

## 4. Bandeja do sistema (Systray)

O Observer fica disponível no ícone da bandeja com o nome **Observer**.

- Clique no ícone e escolha **Abrir** para voltar à tela de status.
- Use essa área para acesso rápido sem interromper seu trabalho.

---

## 5. Configurações

Você pode acessar **Menu → Configurações** a qualquer momento.

### 5.1. Aba “Credenciais”

Mostra os dados cadastrados:

- **Responsável pela Integração**: CNPJ (não editável após salvar)
- **Estabelecimento**: CNPJ, e-mail, telefone, loja e PDV ID

> Observação: CNPJ e PDV ID ficam bloqueados depois de cadastrados.

### 5.2. Aba “Monitoramento”

Permite alterar a pasta monitorada e enviar histórico:

- **Diretório de monitoramento**: escolha a pasta onde ficam os XMLs.
- **Enviar histórico XML**: varre a pasta e envia todos os XMLs ainda não enviados.

### 5.3. Aba “Geral”

Configurações de sistema e aparência:

- **Iniciar com o sistema**: inicia o Observer automaticamente ao ligar o computador.
- **Customização de cores**: escolha a cor **primária** e **secundária** da interface.
- **Redefinir configurações**: apaga tudo e reinicia o app.

---

## 6. Como o envio de XML funciona

- O Observer lê automaticamente os arquivos `.xml` da pasta monitorada.
- O app mantém um histórico interno para não reenviar o mesmo XML.

---

## 7. Dúvidas rápidas

**O que fazer logo após a instalação?**
- Reinicie a aplicação, assim todas as configurações serão aplicadas corretamente.

**O aplicativo fechou e parou?**
- Não. Ele continua rodando na bandeja do sistema.

**Posso trocar a pasta monitorada?**
- Sim, em Configurações → Monitoramento.

**Preciso informar o CNPJ da Software House?**
- Se não tiver, pode deixar vazio e clicar em SALVAR (Embed será usada).

---

Se precisar de suporte, entre em contato com sua Responsável pela Integração ou com a equipe responsável pelo Observer.

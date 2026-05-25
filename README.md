# Observer v1.0.15 — Manual do Usuário

Este guia descreve o funcionamento do Observer, a aplicação que monitora um diretório de XMLs fiscais e envia os arquivos automaticamente para a plataforma Embed.

---

## 1. Visão geral

O Observer monitora um diretório de XMLs fiscais e envia os arquivos para o backend da Embed.
Ele foi feito para rodar em segundo plano, com acesso rápido pela bandeja do sistema.

O aplicativo mantém um índice local dos arquivos já enviados para evitar reenvios.
Quando o app é reiniciado, ele retoma automaticamente o envio dos XMLs restantes no diretório monitorado.

---

## 2. Primeiro acesso (Setup)

O primeiro acesso ao Observer passa por etapas de configuração guiada.

### 2.1. Tela “SOFTWARE HOUSE”

Informe o **CNPJ da Software House** responsável pela sua integração.

- Se não tiver o CNPJ, clique em **SALVAR** para usar o padrão Embed.
- Se informar um CNPJ, o Observer valida automaticamente.

Ações disponíveis:
- **SALVAR**: valida o CNPJ e avança.
- **SAIR**: fecha o aplicativo.

### 2.2. Tela “ESTABELECIMENTO COMERCIAL”

Informe os dados do estabelecimento:

- **CNPJ**
- **E-mail**
- **Telefone**
- **Loja (opcional)**: apelido do caixa/PDV.

O app identifica automaticamente o **PDV ID** da máquina quando possível.

Ações disponíveis:
- **SALVAR**: registra o estabelecimento.
- **SAIR**: fecha o aplicativo.

### 2.3. Tela “CONFIRMAÇÃO”

Quando necessário, um **código de 4 dígitos** é enviado por e-mail.
Digite o código e clique em **SALVAR** para confirmar o PDV.

Ações disponíveis:
- **SALVAR**: confirma o PDV.
- **SAIR**: fecha o aplicativo.

### 2.4. Tela “MONITORAMENTO”

Selecione a pasta onde os XMLs estão salvos.

- Clique em **BUSCAR** e escolha o diretório.
- Clique em **SALVAR** para ativar o monitoramento.

### 2.5. Tela “MONITORAMENTO ATIVADO”

O app confirma que o monitoramento foi iniciado.
Clique em **INICIAR** para acessar a tela principal.

---

## 3. Tela principal (Status)

A tela principal mostra o status do processamento.

Mensagens típicas:
- **Aguardando arquivo para processamento**
- **Arquivo X sendo processado**
- **Envio concluído**

O app continua rodando na bandeja mesmo quando a janela é fechada.

---

## 4. Bandeja do sistema (Systray)

O Observer fica disponível no ícone da bandeja.

- Clique em **Abrir** para voltar à tela principal.
- A bandeja permite acessar o app sem interromper outras tarefas.

---

## 5. Configurações

Em **Menu → Configurações** você encontra:

### Credenciais

- **Software House**: CNPJ (não editável após salvar).
- **Estabelecimento**: CNPJ, e-mail, telefone, loja e PDV ID.

### Monitoramento

- **Diretório de monitoramento**: escolha a pasta de XMLs.
- **Enviar histórico XML**: envia todos os XMLs que ainda não foram processados.

### Geral

- **Iniciar com o sistema**: abre o Observer automaticamente ao ligar o computador.
- **Customização de cores**: escolha a cor primária e secundária da interface.
- **Redefinir configurações**: apaga as configurações salvas e reinicia o app.

---

## 6. Como o envio de XML funciona

- O Observer vigia o diretório configurado e envia arquivos `.xml` automaticamente.
- O app mantém um índice local dos XMLs já enviados para não reenviar os mesmos arquivos.
- Se o Observer for fechado ou travar, ele retoma o envio dos arquivos restantes na próxima inicialização.

---

## 7. Dúvidas rápidas

**O aplicativo fechou e parou?**
- O app retoma o monitoramento na bandeja quando for aberto novamente.

**Posso trocar a pasta monitorada?**
- Sim, em Configurações → Monitoramento.

**Preciso informar o CNPJ da Software House?**
- Não. Se não tiver, deixe vazio e clique em SALVAR. O Embed será usado por padrão.

---

Se precisar de suporte, entre em contato com a sua Software House ou com a equipe responsável pelo Observer.

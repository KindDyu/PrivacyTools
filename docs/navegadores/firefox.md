# [Firefox](https://firefox.com/)
**Firefox Browser** é um navegador de código aberto e independente (com seu próprio motor, o Gecko), conhecido por ser altamente personalizável e oferecer um equilíbrio entre privacidade, extensões e uso para o usuário geral.

<details>
<summary><strong>Configuração recomendada do Firefox</strong></summary><p align="left">

Essas opções podem ser encontradas em ☰ → Configurações.

## Pesquisar

- [ ] Desmarcar **Sugestões de mecanismos de pesquisa**

## Privacidade e Segurança
### Proteção aprimorada contra rastreamento
- [x] Selecione **Rigoroso** em _Proteção aprimorada contra rastreamento_

Isso protege você bloqueando rastreadores de mídia social, scripts de impressão digital (observe que isso não protege você de _todas_ as impressões digitais), criptomineradores, cookies de rastreamento entre sites e algum outro conteúdo de rastreamento. O ETP protege contra muitas ameaças comuns, mas não bloqueia todos os caminhos de rastreamento porque foi projetado para ter impacto mínimo ou nenhum na usabilidade do site.

### Dados de navegação
Se você quiser permanecer conectado a sites específicos, poderá permitir exceções em **Dados de navegação → Gerenciar exceções...**
- [x] Selecione **Limpar cookies e dados de sites sempre que fechar o Firefox**

Isto protege-o de cookies persistentes, mas não o protege contra cookies adquiridos durante qualquer sessão de navegação. Quando isso estiver ativado, será possível limpar facilmente os cookies do seu navegador simplesmente reiniciando o Firefox. Você pode definir exceções por site, se desejar permanecer conectado a um site específico que visita com frequência.

### DNS sobre HTTPS
- [x] Selecione **Personalizado** em _Escolher provedor_ escolha um provedor adequado

O **Personalizado** impõe o uso de DNS sobre HTTPS, e um aviso de segurança será exibido se o Firefox não conseguir se conectar ao seu resolvedor de DNS seguro ou se o seu resolvedor de DNS seguro disser que os registros do domínio que você está tentando acessar não existem. Isso impede que a rede à qual você está conectado faça o downgrade secreto da segurança do seu DNS.

### Conexão e segurança de software
- [x] Selecione **Ativar o modo somente HTTPS em todas as janelas**

Isso evita que você se conecte involuntariamente a um site em HTTP de texto simples. Sites sem HTTPS são incomuns hoje em dia, então isso deve ter pouco ou nenhum impacto na sua navegação diária.

## Permissões e dados
- [ ] Desmarcar **Enviar dados técnicos e de interação para a Mozilla**
- [ ] Desmarcar **Permitir recomendações personalizadas de extensões**
- [ ] Desmarcar **Permitir que o Firefox execute estudos de funcionalidades**
- [ ] Desmarcar **Permitir que o Firefox melhore funcionalidades, desempenho e estabilidade entre uma atualização e outra**
- [ ] Desmarcar **Enviar ping de uso diário para a Mozilla**
- [ ] Desmarcar **Enviar relatórios de falhas automaticamente**

De acordo com a política de privacidade da Mozilla para o Firefox:
> Firefox sends data about your Firefox version and language; device operating system and hardware configuration; memory, basic information about crashes and errors; outcome of automated processes like updates, safebrowsing, and activation to us. When Firefox sends data to us, your IP address is temporarily collected as part of our server logs.

## Conta e sincronização
### Sincronização
O [Firefox Sync](https://hacks.mozilla.org/2018/11/firefox-sync-privacy) permite que seus dados de navegação (histórico, favoritos, etc.) estejam acessíveis em todos os seus dispositivos e os protege com o E2EE.

Além disso, o serviço Contas Mozilla coleta [alguns dados técnicos](https://mozilla.org/privacy/mozilla-accounts). Se você usar uma conta Mozilla, poderá cancelar:

1. Abra as [configurações do seu perfil](https://accounts.firefox.com/settings#data-collection)
2. Desmarque **Contas Mozilla** em _Coleta e uso de dados_

</p></details>

# Navegadores

## [Tor Browser](https://www.torproject.org/)
**Tor Browser** é um navegador focado em anonimato extremo que utiliza a rede Tor para rotear o tráfego através de múltiplos nós, ocultando o endereço IP e a identidade do usuário de forma muito robusta.

## [Mullvad Browser](https://mullvad.net/browser)
**Mullvad Browser** é uma versão focada em privacidade que importa as tecnologias de "anti-fingerprinting" (anti-impressão digital) do Tor para sua navegação, mas sem o uso da rede Tor, sendo ideal para ser usado com uma VPN ou conexão padrão.

## [Brave](https://brave.com/)
**Brave Browser** é um navegador privado por padrão baseado no Chromium, que bloqueia anúncios e rastreadores de forma nativa, oferecendo uma experiência familiar e com alta compatibilidade com sites.

<details>
<summary><strong>Configuração recomendada Brave Desktop</strong></summary><p align="left">

Essas opções podem ser encontradas em ☰ → Configurações.

## Escudos
Brave inclui algumas medidas anti-impressão digital em seu recurso [Escudos](https://support.brave.com/hc/articles/360022973471-What-is-Shields). Sugiro configurar essas opções [globalmente](https://support.brave.com/hc/articles/360023646212-How-do-I-configure-global-and-site-specific-Shields-settings) em todas as páginas que você visita.

As opções do Escudo podem ser rebaixadas por site, conforme necessário, mas por padrão recomendo definir o seguinte:

- [x] Selecione **Agressivo** em _Rastreadores & bloqueio de anúncios_

<details>
<summary><strong>Usar listas de filtros padrão</strong></summary><p align="left">

O Brave permite que você selecione filtros de conteúdo adicionais na página interna `brave://adblock`. Aconselho não usar esse recurso; em vez disso, mantenha as listas de filtros padrão. Usar listas extras fará com que você se destaque de outros usuários do Brave e também poderá aumentar a superfície de ataque se houver uma exploração no Brave e uma regra maliciosa for adicionada a uma das listas que você usa.

</p></details>

- [x] Selecione **Rigorosa** em _Fazer upgrade das conexões para HTTPS_
- [x] Selecione **Bloquear scripts** (Opcional)
> Esta opção desativa o JavaScript, o que quebrará muitos sites. Para corrigi-los, você pode definir exceções por site clicando no ícone Escudo na barra de endereço e desmarcando essa configuração em _Opções avançados_.
- [x] Verifique **Bloquear impressões digitais**
- [x] Selecione **Bloquear cookies de terceiros**
- [x] Verifique **Esqueça de mim quando fechar este site**
> Se desejar permanecer conectado a um site específico que você visita com frequência, você pode definir exceções por site clicando no ícone Escudo na barra de endereço e desmarcando essa configuração em _Opções avançados_.
- [ ] Desmarque todos os componentes de mídia social

## Privacidade e segurança
- [x] Selecione **Não permitir que os sites usem a otimização de JavaScript** em _Segurança_ → _Gerenciar a otimização e segurança de JavaScript_
> Desativar o otimizador V8 reduz sua superfície de ataque desativando [algumas](https://grapheneos.social/@GrapheneOS/112708049232710156) partes da compilação JavaScript Just-In-Time (JIT).
- [x] Selecione **Remover automaticamente as permissões de sites não usados** em _Configurações de site e segurança (escudos)_
- [x] Selecione **Desativar UDP não proxy** na [Política de manuseio de IP do WebRTC](https://support.brave.com/hc/articles/360017989132-How-do-I-change-my-Privacy-Settings#webrtc)
- [ ] Desmarque **Use os serviços do Google para receber mensagens push**
- [x] Selecione **Redirecionar automaticamente páginas de AMP**
- [x] Selecione **Redirecionar URLs de rastreamento automaticamente**
- [x] Selecione **Impedir que sites criem impressões digitais minhas com base nas minhas preferências de idioma**

### Janelas Tor
[Janela privada com o Tor](https://support.brave.com/hc/articles/360018121491-What-is-a-Private-Window-with-Tor-Connectivity) permite que você roteie seu tráfego pela rede Tor no Private Windows e acesse os serviços .onion, que podem ser úteis em alguns casos. No entanto, o Brave não é tão resistente à impressão digital quanto o navegador Tor, e muito menos pessoas usam o Brave com Tor, então você vai se destacar. Se o seu modelo de ameaça exigir forte anonimato, use o navegador [Tor]().

### Coleta de dados
- [ ] Desmarque **Permitir a análise de produtos com preservação da privacidade (P3A)**
- [ ] Desmarque **Enviar automaticamente um ping diário de uso ao Brave**
- [ ] Desmarque **Enviar relatórios de diagnóstico automaticamente**

## Web3
Os recursos Web3 do Brave podem potencialmente aumentar a impressão digital e a superfície de ataque do seu navegador. A menos que você use algum desses recursos, eles devem ser desativados
- [x] Selecione **Extensões (sem fallback)** em _Carteira Ethereum padrão_
- [x] Selecione **Extensões (sem fallback)** em _Carteira Solana padrão_

## Mecanismo de pesquisa
- [ ] Desmarque **Melhores sugestões de pesquisa**
> As sugestões de pesquisa enviam tudo o que você digita na barra de endereço para o mecanismo de pesquisa padrão, independentemente de você enviar uma pesquisa real. Desativar sugestões de pesquisa permite que você controle com mais precisão quais dados você envia ao seu provedor de mecanismos de pesquisa.

## Extensões
- [ ] Desmarque todas as extensões integradas que você não usa

## Sistema
- [ ] Desmarque **Continuar executando os aplicativos em segundo plano quando o Brave for fechado**
> Esta opção não está presente em todas as plataformas.

### Brave Sync
[Brave Sync](https://support.brave.com/hc/articles/360059793111-Understanding-Brave-Sync) permite que seus dados de navegação (histórico, favoritos, etc.) estejam acessíveis em todos os seus dispositivos sem a necessidade de uma conta e os protege com a criptografia de ponta a ponta.

### Recompensas Brave
**Recompensas Brave** permite que você receba a criptomoeda Basic Attention Token (BAT) por executar determinadas ações no Brave. Ele depende de uma conta de custódia e KYC (Know Your Costumer) de um número selecionado de provedores. Não recomendo o BAT como uma **criptomoeda privada**, nem recomendo o uso de uma **carteira de custódia**, por isso desencorajo o uso desse recurso.

### Carteira Brave
**Carteira Brave** opera localmente no seu computador, mas não oferece suporte a nenhuma criptomoeda privada, por isso desencorajo o uso desse recurso também.

</p></details>

<details>
<summary><strong>Configuração recomendada Brave Mobile</strong></summary><p align="left">

Essas opções podem ser encontradas em ⋮ → Configurações → Proteções do Brave e privacidade.

## Padrões globais do Brave Shields
Brave inclui algumas medidas anti-impressão digital em seu recurso [Escudos](https://support.brave.com/hc/articles/360022973471-What-is-Shields). Sugiro configurar essas opções [globalmente](https://support.brave.com/hc/articles/360023646212-How-do-I-configure-global-and-site-specific-Shields-settings) em todas as páginas que você visita.

As opções do Escudo podem ser rebaixadas por site, conforme necessário, mas por padrão recomendo definir o seguinte:

- [x] Selecione **Agressivo** em _Bloquear rastreadores e anúncios_
- [x] Selecione **Redirecionar automaticamente páginas de AMP**
- [x] Selecione **Redirecionar URLs de rastreamento automaticamente**
- [x] Selecione **Estrito** em _Fazer upgrade das conexões para HTTPS_
- [x] Selecione **Bloquear scripts** (Opcional)
> Esta opção desativa o JavaScript, o que quebrará muitos sites. Para corrigi-los, você pode definir exceções por site clicando no ícone Escudo na barra de endereço e desmarcando essa configuração em _Opções avançados_.
- [x] Selecione **Bloquear cookies de terceiros** em _Bloquear cookies_
- [x] Selecione **Bloquear impressões digitais**
- [x] Selecione **Evite impressões digitais por meio das configurações de idioma**

<details>
<summary><strong>Usar listas de filtros padrão</strong></summary><p align="left">

O Brave permite que você selecione filtros de conteúdo adicionais no menu **Filtragem de conteúdo** ou na página interna `brave://adblock`. Não recomendo o uso desse recurso; em vez disso, mantenha as listas de filtros padrão. O uso de listas adicionais fará com que você se destaque dos demais usuários do Brave e também poderá aumentar a superfície de ataque caso haja uma vulnerabilidade no Brave e uma regra maliciosa seja adicionada a uma das listas que você utiliza.

Traduzido com a versão gratuita do tradutor - DeepL.com

</p></details>

- [x] Selecione **Abas so site fechadas** em _Destruir_

## Outras configurações de privacidade
- [x] Selecione **Sem proteção** em _Navegação Segura_
- [x] Selecione **Desativar UDP não proxy** em [Política de manuseio de IP do WebRTC](https://support.brave.com/hc/articles/360017989132-How-do-I-change-my-Privacy-Settings#webrtc)
- [ ] Desmarque **Permitir que os sites verifiquem se você tem formas de pagamento salvas**
- [x] Selecione **Do no speed up sites with Brave's V8** em _Otimização e segurança de JavaScript_
- [x] Selecione **Fechar as guias ao sair**
- [ ] Desmarque **Enviar relatórios de diagnóstico automaticamente**
- [ ] Desmarque **Enviar automaticamente um ping diário de uso ao Brave**
- [ ] Desmarque **Autorizar pesquisas Brave**

## Leo AI
- [ ] Desmarque **Exibir sugestões de preenchimento automático na barra de endereço**

## Mecanismos de pesquisa
- [ ] Desmarque **Mostrar sugestões de navegador**

</p></details>

## [Firefox](https://firefox.com/)
**Firefox Browser** é um navegador de código aberto e independente (com seu próprio motor, o Gecko), conhecido por ser altamente personalizável e oferecer um equilíbrio entre privacidade, extensões e uso para o usuário geral.

- [Configuração recomendada Firefox](/SPA/navegação-na-internet/config-firefox.md)

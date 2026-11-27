# MnzPlay

Portal web de jogos e emulação em arquivo único (`index.html`), com catálogo interativo, suporte a controle no menu principal, sistema de amigos no estilo Steam, chat com persistência na nuvem e integração com **Supabase**.

## Recursos

* **Catálogo e navegação:** abas de *Jogos*, *Favoritos* e *Recentes*, busca instantânea e filtro por sistema (*N64*, *SNES*, *Web / JS*).
* **Mídia física 3D:** giro frente e verso com detalhes do jogo e possibilidade de personalizar frente e verso localmente no navegador.
* **Emulação no navegador:** execução via *EmulatorJS* (com suporte a carregamento de ROMs locais pelo botão **ROM**) e atalhos para links/ports web.
* **Controle (Gamepad API):** navegação por D-Pad/analógico, atalhos de botões, deadzone configurável e indicadores de status na barra superior.
* **Amigos e chat na nuvem:** lista de amigos por status (*Em jogo*, *Online*, *Offline*), presença de jogo atual e mensagens salvas no **Supabase** com cache local em `localStorage`.

## Arquitetura e Backend

* **Frontend:** `index.html` autocontido (HTML, CSS e JavaScript).
* **Supabase:** autenticação, tabela de perfis (`perfis`) e persistência de mensagens (`mensagens`).

## Hospedagem

* **GitHub Pages:** publicado a partir da branch `main` na raiz (`/ (root)`).
* **Cloudflare Pages:** espelho/hospedagem estática conectada ao repositório para redundância.

## Aviso sobre ROMs

As ROMs não são distribuídas junto ao repositório; utilize o botão **ROM** dentro do player para carregar seus próprios arquivos (`.z64`, `.n64`, `.v64`, `.sfc`, `.smc`) diretamente no navegador.

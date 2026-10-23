# Mundo Vivo — versão PWA

Esta pasta contém uma versão instalável do jogo, com os recursos locais guardados para funcionar offline depois de carregada.

## Abrir o jogo

O PWA precisa ser aberto por `localhost` ou por um site HTTPS. Não abra `index.html` diretamente como `file://`.

No Windows, abra um terminal nesta pasta e execute:

```powershell
py -m http.server 8000
```

Se o comando `py` não existir, tente:

```powershell
python -m http.server 8000
```

Depois visite [http://localhost:8000](http://localhost:8000).

## Instalar

- **Chrome ou Edge no computador:** use o ícone Instalar na barra de endereço ou o menu do navegador → **Instalar Mundo Vivo**.
- **Android:** abra no Chrome e escolha **Instalar app** ou **Adicionar à tela inicial**.
- **iPhone/iPad:** abra no Safari, toque em **Compartilhar** e escolha **Adicionar à Tela de Início**.

Na primeira abertura, aguarde o jogo carregar e o navegador registrar o cache. Depois disso, o jogo pode ser iniciado sem conexão pela instalação.

## Arquivos

- `index.html`: jogo.
- `manifest.webmanifest`: nome, ícones e apresentação do aplicativo.
- `sw.js`: cache offline e atualização do app shell.
- `vendor/three.min.js`: Three.js r128, empacotado para uso offline.
- `vendor/THREE-LICENSE.txt`: licença do Three.js.

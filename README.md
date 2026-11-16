# Missão Reciclagem

Jogo educativo de reciclagem para navegador, com cenários 3D, narração em português brasileiro e opções de personalização do personagem.

## Jogar

https://gustavo-ferreira03.github.io/missao-reciclagem/

O jogo também pode ser aberto diretamente pelo arquivo `index.html`. Os recursos do jogo estão incorporados ao HTML.

## Publicação

GitHub Pages publica a raiz da branch `main`. Para atualizar o jogo, substitua `index.html` pela nova versão.

## Estatísticas

O jogo pede autorização antes de enviar eventos de interação e gravações visuais da tela ao PostHog. É possível jogar sem autorizar. O botão Privacidade (escudo, no topo) permite alterar a escolha; retirar a autorização interrompe novos registros e descarta a fila local, sem apagar dados já enviados. A escolha fica salva neste navegador quando o armazenamento está disponível. O aviso de autorização é dirigido ao responsável. O envio precisa de internet. O sinal GPC não bloqueia uma coleta autorizada. Do Not Track e `?analytics=off` continuam desativando a coleta. Os testes usam `?analytics_test=1`.

Para diagnóstico, execute no console do navegador:

```js
await GameAnalytics.flush();
GameAnalytics.status();
```

A configuração incorporada contém apenas o token público de captura do projeto. Nenhuma credencial privada é necessária no site.

# Missão Reciclagem

Jogo educativo de reciclagem para navegador, com cenários 3D, narração em português brasileiro e opções de personalização do personagem.

## Jogar

https://gustavo-ferreira03.github.io/missao-reciclagem/

O jogo também pode ser aberto diretamente pelo arquivo `index.html`. Os recursos do jogo estão incorporados ao HTML.

## Publicação

GitHub Pages publica a raiz da branch `main`. Para atualizar o jogo, substitua `index.html` pela nova versão.

## Estatísticas

O jogo usa PostHog para eventos de interação e gravação de sessões. O envio precisa de internet. O sinal GPC não bloqueia a coleta. Do Not Track e `?analytics=off` desativam a coleta. Os testes usam `?analytics_test=1`.

Para diagnóstico, execute no console do navegador:

```js
await GameAnalytics.flush();
GameAnalytics.status();
```

A configuração incorporada contém apenas o token público de captura do projeto. Nenhuma credencial privada é necessária no site.

## Angular Routing

Em uma aplicação single-page, você muda o que o usuário vê mostrando ou escondendo porções do display que
corresponde a componentes particulares, em vez de r para o servidor para pegar uma página nova. Conforme usuários
performam tarefas na aplicação, eles precisam se mover entre as diferentes <b>views</b> que você definiu.

Para lidar com a navegação de uma <b>view</b> para a próxima, você usa o ``Router`` do Angular. O ``Router`` habilita a 
navegação interpretando a URL do navegador como uma instrução para mudar a <b>view</b>.
<hr>


### Definindo um roteador básico 

Há três blocos de construções fundamentais para criar um route.<br>

Importe o roteador para ``app.config.ts`` e adicione isso a função ``providerRouter``.<br>

O Angular CLI faz esse passo para você. Mas, de qualquer jeito, se você está criando uma aplicação manualmente

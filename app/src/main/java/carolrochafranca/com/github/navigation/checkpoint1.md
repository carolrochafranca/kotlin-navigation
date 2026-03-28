Professor, segue a explicação do que foi feito nos últimos 4 commits do projeto sobre navegação com Jetpack Compose:

1. Passagem de parâmetros obrigatórios na tela de Perfil
   Nesse primeiro commit, a ideia foi fazer a tela de Perfil receber uma informação da tela anterior (no caso, o nome do usuário). Para isso, mudei a rota na MainActivity de "perfil" para "perfil/{nome}". A função da PerfilScreen foi ajustada para exigir a String do nome e mostrá-la na tela. Lá na MenuScreen, atualizei o clique do botão para mandar esse dado direto na string de navegação: Maps("perfil/Fulano de Tal").

2. Passagem de parâmetros opcionais na tela de Pedidos
   Aqui o objetivo foi um pouco diferente: passar dados, mas sem obrigar a tela a recebê-los para funcionar. Na MainActivity, mudei a rota da tela de Pedidos para usar query parameters, ficando "pedidos?cliente={cliente}". O detalhe importante aqui foi usar o navArgument para definir um valor padrão ("Cliente Genérico"). Dessa forma, se a tela for aberta sem receber o nome do cliente, o app não quebra e exibe o valor padrão. A PedidosScreen foi atualizada para receber esse cliente e mostrar no Text.

3. Inserindo valor ao parâmetro opcional na tela de Pedidos
   Esse commit foi bem direto, serviu basicamente para testar e usar a estrutura criada no commit anterior. Fui no botão da MenuScreen e mudei a ação de navegação para enviar de fato um parâmetro. A chamada passou a ser Maps("pedidos?cliente=Cliente XPTO"). Com isso, a tela de pedidos passou a exibir "Cliente XPTO" no lugar do valor genérico.

4. Passagem de múltiplos parâmetros
   Por fim, evoluí a tela de Perfil para receber mais de um dado, e de tipos diferentes. A rota na MainActivity mudou para "perfil/{nome}/{idade}". Para evitar problemas, declarei explicitamente os tipos usando o NavType (o nome como StringType e a idade como IntType). O botão no menu passou a mandar a idade junto ("perfil/Fulano de Tal/27"), e a PerfilScreen foi atualizada para receber esse Int e mostrar a frase completa formatada com os dois dados.

Resumindo: Os commits mostram a evolução da navegação no app, começando com rotas simples e terminando com rotas que conseguem receber múltiplos parâmetros tipados (obrigatórios) e parâmetros de busca (opcionais com valor padrão).
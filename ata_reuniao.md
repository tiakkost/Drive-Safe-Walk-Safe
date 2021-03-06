#Drive-Safe-Walk-Safe

## Ata de Reunião

Data         | Local
------------ | -------------
13/04/2017   | (Entrevista remota)


### Participantes
* Hiroito Miyakawa
* Paulo Marques
* Paulo Vaz (PO/GP)
* Roberto Pires (Cliente)
* Samuel Paes
* Valdir Souza

### Objetivos
* Fazer reunião com o cliente para obter ao menos uma visão geral de como se deseja que o sistema seja implementado.

### Tópicos Discutidos
* Objetivo da implementação do sistema;
* Estrutura de páginas;
* Quais dados serão armazenados e como serão armazenados;
* Como as informações serão exibidas.

### Ações a serem tomadas
Ação                                | Responsável   
----------------------------------- | ----------------
Iniciar implementação de protótipos | Todos da equipe
Estudar Ruby, Rails e as plataformas a serem utilizadas | Todos da equipe
Fazer mockup (Lo-Fi) da página principal | Paulo Vaz
Fazer mockup (Lo-Fi) da janela de comentário | Samuel Paes
Fazer mockup (Lo-Fi) da página de recomendações e precauções | Paulo Marques

###Informações Adicionais
* Entrevista:
1) Descreva o objetivo do sistema.
R: O sistema Drive Safe, Walk Safe deve exibir dados em forma de texto e de gráficos para o público aberto, de forma a conscientizar quem acesse sobre a importância de ser prudente no trânsito para que não façam parte das estatísticas exibidas no sistema. Os usuários devem poder filtrar os dados, também. E seria um bom extra incluir algumas dicas sobre como evitar acidentes.

2) Haverá algum dado armazenado em banco de dados?
R: Os dados serão coletados da base de dados abertos http://dados.recife.pe.gov.br/dataset/acidentes-de-transito-com-e-sem-vitimas e armazenados em banco para serem disponibilizados ao usuário. Além disso, os usuários poderão fazer comentários a respeito das ocorrências exibidas individualmente, se desejarem. Usuários podem acessar informações sobre acidentes individualmente ou num contexto geral (gráficos).

3) Quais ações são esperadas do usuário ao utilizar o sistema?
R: O usuário poderá acessar informações individuais de um acidente de trânsito, num pop-up. Poderá visualizar gráficos com estatísticas filtradas pelo próprio usuário. Espera-se que haja filtros de período (data inicial e final), acidentes com ou sem vítimas, localização e tipo de veículo, a princípio.  Além disso, o usuário poderá, ao visualizar as informações visuais de um acidente, adicionar comentários neste.

4) O sistema precisará controlar logins de usuários?
R: Usuários não terão login. O sistema será aberto. Os comentários não serão associados a usuários, no banco de dados.

5) Como será a estrutura de páginas do sistema?
R: A página principal terá o nome “Consulta” e exibirá, por padrão, informações sobre acidentes no mês vigente e no mesmo período em anos anteriores, em formato de gráfico e de tabela. Se o usuário modificar os filtros, os gráficos e tabelas também mudarão. Numa pesquisa cujo resultado traga itens individuais de acidentes, o usuário pode clicar num ícone (cada linha terá seu ícone) para exibir um pop-up onde poderão ser vistos detalhes sobre o acidente e onde o usuário poderá inserir seus comentários.
Haverá uma outra página onde serão exibidas as dicas sobre como evitar acidentes de trânsito em formato textual e com o auxílio de imagens.

6) O sistema deve se integrar com alguma API?
R: Sim. O sistema deve permitir o usuário visualizar o local do acidente no Google Maps, com o auxílio de sua API.

7) Mais alguma observação, exigência ou preferência?
R: Gostaria que o sistema fosse fácil de manusear, sem clicks desnecessários. Sua estrutura e funcionalidade são simples, então espera-se que o usuário tenha essa experiência. Seria bom fazer com o que a aparência do sistema seja agradável, para que os usuários o acessem de qualquer dispositivo e tenham uma visão agradável.

8) Quais campos devem haver na janela de comentários?
R: Os campos são: Nome, Email e Descrição. A descrição é o comentário em si.

# Exercício Prático - eSports

## Descrição

Você foi contratado por uma empresa de jogos para desenvolver um sistema de gerenciamento de um torneio de eSports. Esse sistema deve ser capaz de gerenciar os jogadores, os times, os jogos e as competições. Cada jogador pode pertencer a um time, e cada time pode participar de várias competições. Cada competição tem várias partidas entre os times, e cada partida tem um resultado específico.

O objetivo do sistema é facilitar a organização e a visualização de informações relacionadas ao torneio, incluindo o registro de novos jogadores, a formação de times, a criação de competições e o registro dos resultados das partidas.

## Elementos do Sistema

### 1. `Jogador`

- `id`: Identificador
- `nome`: Representa o nome completo do jogador.
- `nickname`: Representa o apelido ou nome de usuário do jogador.
- `idade`: Idade do jogador.
- `posicao`: A posição que o jogador ocupa no time (por exemplo, atacante, defensor).

### 2. `Time`

- `id`: Identificador
- `nomeTime`: O nome do time.
- `pais`: País de origem do time.
- `jogadores`: Lista de jogadores que fazem parte do time.
- `treinador`: Nome do treinador do time.

### 3. `Partida`

- `id`: Identificador
- `dataPartida`: Data e hora em que a partida será realizada.
- `timeA`: Referência ao primeiro time participante da partida.
- `timeB`: Referência ao segundo time participante da partida.
- `pontuacaoTimeA`: Pontuação obtida pelo primeiro time.
- `pontuacaoTimeB`: Pontuação obtida pelo segundo time.

### 4. `Competicao`

- `id`: Identificador
- `nomeCompeticao`: Nome da competição.
- `dataInicio`: Data de início da competição.
- `dataFim`: Data de término da competição.
- `timesParticipantes`: Lista de times inscritos na competição.
- `partidas`: Lista de partidas programadas para a competição.

## Elementos do Sistema

- `Registrar Novo Jogador`: Adicionar um novo jogador ao sistema com informações como nome, nickname, idade e posição.
- `Atualizar Informações do Jogador`: Modificar os dados pessoais do jogador, como nome, nickname ou posição.
- `Visualizar Informações do Jogador`: Exibir os detalhes do jogador.
- `Criar Novo Time`: Registrar um novo time no sistema com um nome e uma lista inicial de jogadores.
- `Adicionar Jogador ao Time`: Incluir um jogador existente em um time específico.
- `Remover Jogador do Time`: Excluir um jogador de um time. Esta ação retira um jogador de um time, mas não remove o jogador do sistema.
- `Visualizar Detalhes do Time`: Exibir informações completas sobre o time, incluindo lista de jogadores e competições em que está inscrito.
- `Agendar Partida`: Programar uma nova partida entre dois times para uma data e hora específicas. Define uma nova partida no calendário, incluindo detalhes de data, hora e times participantes.
- `Registrar Resultado da Partida`: Inserir o resultado de uma partida após seu término. Permite o registro das pontuações de cada time após a conclusão da partida.
- `Visualizar Histórico de Partidas`: Mostrar todas as partidas agendadas ou já realizadas, com seus respectivos resultados. Exibe um histórico completo das partidas, incluindo vencedores.
- `Criar Competição`: Iniciar uma nova competição, definindo seu nome, datas e times participantes.
- `Adicionar Time à Competição`: Inscrever um time em uma competição. Permite a inscrição de um time em uma competição já existente.
- `Remover Time da Competição`: Excluir um time da lista de participantes de uma competição. Esta ação remove um time de uma competição específica, mas não do sistema.
- `Gerar Relatório da Competição`: Criar um relatório detalhado da competição, incluindo partidas, resultados e classificação final.

OBS.: Todas as entidades devem ter um identificador

# JunkBox

Protótipo de uma interface gráfica para um aplicativo de músicas, feito em Python com Pygame. O projeto reúne telas de acesso, pesquisa, playlists, seleção do modo de reprodução e upload de arquivos.

## Requisitos

- Python 3.10 ou superior
- Pygame

## Como executar

1. Clone o repositório e entre na pasta do projeto.
2. Instale a dependência:

   ```bash
   python -m pip install pygame
   ```

3. Inicie o aplicativo:

   ```bash
   python JunkBox.py
   ```

## Navegação

- **Tela inicial:** permite abrir o login, o cadastro ou sair.
- **Login e cadastro:** exibem campos de e-mail e senha. O fluxo é demonstrativo; não há autenticação ou persistência de usuários.
- **Menu principal:** dá acesso à pesquisa, playlists, upload e seleção do modo de reprodução.
- **Pesquisa:** recebe texto, mas ainda não consulta uma biblioteca de músicas.
- **Playlists:** permite iniciar o fluxo de criação; acessar playlists existentes ainda não está implementado.
- **Modo de reprodução:** apresenta as opções aleatória e sequencial, sem reproduzir áudio.
- **Upload:** o botão de carregamento é apenas ilustrativo; não abre nem armazena arquivos.

## Estrutura do projeto

| Arquivo | Responsabilidade |
| --- | --- |
| `JunkBox.py` | Inicializa e executa o loop principal da aplicação. |
| `window.py` | Configura o Pygame, a janela e as dimensões da tela. |
| `statemachine.py` | Mantém o estado atual e controla a navegação entre telas. |
| `initialmenu.py`, `login.py`, `cadastro.py` | Telas inicial, de login e de cadastro. |
| `mainmenu.py`, `search.py`, `playlists.py` | Menu principal, pesquisa e fluxo de playlists. |
| `selectrepro.py`, `upload.py` | Seleção de reprodução e tela de upload. |
| `button.py`, `TextInput.py`, `text.py` | Componentes reutilizáveis de interface. |

## Estado atual

O repositório implementa a navegação e os componentes visuais básicos. Recursos de produto — como autenticação, busca real, armazenamento de playlists, seleção de arquivos e reprodução de áudio — ainda precisam ser conectados ou implementados.

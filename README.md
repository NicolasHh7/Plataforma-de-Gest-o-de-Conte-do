# Plataforma de Gestão de Conteúdo
client/
├── src/
│   ├── assets/            # Imagens e ícones
│   ├── scss/              # Estilização organizada
│   │   ├── main.scss      # Arquivo central (importa os outros)
│   │   ├── _variables.scss # Cores, fontes e espaçamentos
│   │   ├── _mixins.scss   # Atalhos CSS
│   │   └── _dashboard.scss # Estilos específicos do painel
│   ├── ts/                # Lógica em TypeScript
│   │   ├── api.ts         # Chamadas fetch para o Node.js
│   │   ├── auth.ts        # Lógica de login/sessão
│   │   └── editor.ts      # Manipulação do Markdown/HTML
│   └── index.html         # Página principal (Home/Blog)
│   └── admin.html         # Painel de controle do autor
├── package.json
└── tsconfig.json

server/
├── src/
│   ├── controllers/       # Lógica das rotas (ex: postController.ts)
│   ├── models/            # Estrutura dos dados (ex: Post.ts)
│   ├── routes/            # Definição dos caminhos da API (ex: authRoutes.ts)
│   ├── middlewares/       # Filtros (ex: verificar se o usuário é admin)
│   ├── services/          # Regras de negócio (ex: conversão de Markdown)
│   └── index.ts           # Ponto de entrada do servidor Express
├── data/                  # Onde os arquivos JSON ou DB residirão
├── package.json
└── tsconfig.json
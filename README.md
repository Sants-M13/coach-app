# coach-app — superfície de captura de treino do coach-os

Web app estático (HTML puro, zero build) pra registrar treino no celular durante a sessão:
séries, carga, timer de descanso (com som/vibração/wake lock). Ao finalizar, commita a sessão
como JSON no repo privado `coach-os` via API do GitHub (PAT fine-grained salvo só no localStorage).

- Plano de treino: carregado de `coach-os/treino/planos/current.json` (privado, via PAT); fallback embutido.
- Log: `coach-os/treino/logs/AAAA-MM/AAAA-MM-DD-<dia>.json`.
- **Este repo é só código — nenhum dado pessoal vive aqui.**

Uso: abrir a página do GitHub Pages no celular → ⚙ → colar o PAT (Contents read/write só no coach-os) → treinar.

# Trabalho 5 — Pipeline CI Mínimo e Reprodutível

## 📋 Identificação dos Elementos do Pipeline
- **Gatilho (Trigger):** Disparado automaticamente ao realizar um `push` ou abrir um `pull_request` nas branches `main` ou `master`.
- **Etapas (Stages):**
  1. Checkout do código
  2. Configuração do ambiente de execução (Node.js)
  3. Instalação de dependências (`npm ci`)
  4. Execução de testes
  5. Build da aplicação
  6. Geração e armazenamento de artefato
- **Dependências:** Gerenciadas via `npm` através do `package.json` e `package-lock.json`[cite: 2].
- **Artefato:** Gerado ao final do build e disponibilizado na aba *Actions* do GitHub com o identificador correspondente ao commit (`build-artifact-<COMMIT_SHA>`)[cite: 2].

---

## 🛠️ Como Reproduzir Localmente
1. Clone este repositório[cite: 2]:
   ```bash
   git clone [https://github.com/CriminalBR/ProjetoCloud.git](https://github.com/CriminalBR/ProjetoCloud.git)
   cd ProjetoCloud

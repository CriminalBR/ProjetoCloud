# Trabalho 5 — Pipeline CI Mínimo e Reprodutível

## 📋 Identificação dos Elementos do Pipeline
- **Gatilho (Trigger):** Disparado automaticamente ao realizar um `push` ou abrir um `pull_request` nas branches `main` ou `master`.
- **Etapas (Stages):**
  1. Checkout do código
  2. Configuração do ambiente de execução
  3. Instalação de dependências
  4. Execução de testes
  5. Build da aplicação
  6. Geração e armazenamento de artefato
- **Dependências:** Gerenciadas via `npm` (ou equivalente da linguagem).
- **Artefato:** Gerado ao final do build e disponibilizado na aba *Actions* com o identificador `build-artifact-<COMMIT_SHA>`.

---

## 🛠️ Como Reproduzir Localmente
1. Clone este repositório:
   ```bash
   git clone <https://github.com/CriminalBR/ProjetoCloud.git>
   cd <ProjetoCloud>

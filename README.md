# 💻 Backup das Configurações do VSCode

Este repositório contém minhas configurações personalizadas do **Visual Studio Code**, permitindo que eu as recupere facilmente ao trocar de máquina ou reinstalar o editor.

## 📂 O que está incluído?
- **settings.json** → Configurações gerais do editor.
- **extensions.json** → Lista de extensões instaladas.
- **keybindings.json** → Atalhos personalizados.
- Outros arquivos relevantes para manter o ambiente de desenvolvimento consistente.

## 🚀 Como restaurar as configurações?

### 🔹 1. Clonar o repositório
```bash
git clone https://github.com/seu-usuario/vscode-settings.git
cd vscode-settings
```

### 🔹 2. Copiar as configurações para o VSCode
```bash
cp settings.json "$HOME/.config/Code/User/"  # Linux
cp settings.json "%APPDATA%\Code\User\"  # Windows
cp settings.json "~/Library/Application Support/Code/User/"  # macOS
```

### 🔹 3. Restaurar extensões
```bash
cat extensions.json | xargs -n1 code --install-extension
```

## 📌 Como atualizar as configurações?
Sempre que fizer ajustes no VSCode e quiser salvar no repositório:
```bash
git add .
git commit -m "chore(vscode): atualiza settings do VSCode"
git push origin main
```

## 🎯 Recomendações
- Utilize este repositório como um **backup pessoal**.
- Se precisar sincronizar automaticamente, pode usar o **Settings Sync** do VSCode.

---
**Mantenha suas configurações sempre seguras! 🚀**

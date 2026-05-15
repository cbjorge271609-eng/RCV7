# RC Financeiro — Sistema Financeiro RC Comunicação Visual

App financeiro PWA (Progressive Web App) para iOS/Android/Desktop.

---

## 📁 Estrutura de Arquivos

```
rc-financeiro/
├── index.html       ← App completo (tudo em 1 arquivo)
├── manifest.json    ← Configuração do PWA
├── sw.js            ← Service Worker (modo offline)
├── icons/
│   ├── icon-180.png ← Apple Touch Icon (iPhone)
│   ├── icon-167.png ← Apple Touch Icon (iPad Pro)
│   ├── icon-152.png ← Apple Touch Icon (iPad)
│   ├── icon-120.png ← Apple Touch Icon (iPhone menor)
│   ├── icon-192.png ← Android / PWA
│   └── icon-512.png ← Splash screen
└── README.md
```

---

## 🚀 Como publicar no GitHub Pages (passo a passo)

### 1. Criar repositório no GitHub
1. Acesse **github.com** e faça login
2. Clique em **"New repository"** (botão verde)
3. Nome sugerido: `rc-financeiro`
4. Deixe como **Public**
5. Clique em **"Create repository"**

### 2. Fazer upload dos arquivos
**Opção A — Interface Web (mais fácil):**
1. No repositório criado, clique em **"uploading an existing file"**
2. Arraste todos os arquivos desta pasta (index.html, manifest.json, sw.js)
3. Arraste também a pasta `icons/` com todos os ícones
4. Clique em **"Commit changes"**

**Opção B — Git no terminal:**
```bash
git init
git add .
git commit -m "RC Financeiro v1.0"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/rc-financeiro.git
git push -u origin main
```

### 3. Ativar GitHub Pages
1. No repositório, vá em **Settings** (engrenagem)
2. No menu lateral, clique em **Pages**
3. Em "Source", selecione **"Deploy from a branch"**
4. Branch: **main** / Folder: **/ (root)**
5. Clique em **Save**
6. Aguarde 1-2 minutos
7. Seu app estará em: `https://SEU_USUARIO.github.io/rc-financeiro/`

---

## 📱 Instalar no iPhone como App (iOS PWA)

1. Abra o **Safari** no iPhone (obrigatório — Chrome não instala PWA no iOS)
2. Acesse: `https://SEU_USUARIO.github.io/rc-financeiro/`
3. Toque no ícone de **compartilhar** (quadrado com seta para cima)
4. Role a lista e toque em **"Adicionar à Tela de Início"**
5. Confirme o nome "RC Fin" e toque em **"Adicionar"**
6. O ícone aparecerá na tela como um app nativo ✅

---

## ✅ Funcionalidades

- 📊 **Dashboard** com KPIs automáticos: Receita, Despesas, Lucro, Markup, EBITDA
- 💰 **Receitas** — lançamento com nº orçamento, cliente, valor, status
- 💳 **Despesas** — custos fixos (lançamento rápido) + despesas livres com anexo de comprovante
- 👥 **Clientes** — ranking por receita gerada com ticket médio
- 📈 **Relatórios / DRE** — demonstrativo mês a mês
- ⚙️ **Configurações** — dados da empresa e custos fixos de referência
- 📶 **Offline** — funciona sem internet (Service Worker)
- 💾 **Dados salvos localmente** — localStorage (por dispositivo)

---

## ⚠️ Importante — Dados Locais

Os dados ficam salvos no **localStorage do navegador**, ou seja:
- Ficam no dispositivo onde foram lançados
- Não sincronizam entre dispositivos automaticamente
- **Não se perdem ao fechar o app**
- Se limpar o cache do Safari, os dados são apagados

### Para sincronização entre dispositivos (versão futura):
Será necessário adicionar um backend (Supabase, Firebase ou similar) para banco de dados em nuvem. Consulte o desenvolvedor quando quiser evoluir para isso.

---

## 📞 Suporte
Cristiano Bernardo Jorge — RC Comunicação Visual
CNPJ: 61.457.178/0001-50 — Serra, ES

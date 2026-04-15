# 📤 COMO SUBIR PARA O GITHUB

## Passo a Passo Rápido (5 minutos)

### 1. Inicialize o Git (se ainda não fez)
```bash
cd gstd-operacional
git init
```

### 2. Adicione Todos os Arquivos
```bash
git add .
```

### 3. Faça o Primeiro Commit
```bash
git commit -m "🚀 Initial commit - GSTD Operacional MVP"
```

### 4. Conecte com Repositório Remoto
```bash
git remote add origin https://github.com/gstd-ag/crm-new.git
```

### 5. Suba para o GitHub
```bash
git branch -M main
git push -u origin main
```

---

## 🔗 Link do Repositório

**Repositório Oficial:** https://github.com/gstd-ag/crm-new

---

## ✅ Checklist de Upload

- [ ] `README.md` - Documentação principal
- [ ] `SCRIPTS_WHATSAPP.md` - Scripts de vendas
- [ ] `GUIA_IMPLANTACAO.md` - Guia passo a passo
- [ ] `src/` - Código fonte React
- [ ] `public/` - Assets estáticos
- [ ] `package.json` - Dependências
- [ ] `.gitignore` - Arquivos ignorados
- [ ] `index.html` - Entry point
- [ ] Configs (tailwind, vite, eslint)

---

## ⚠️ O Que NÃO Subir

- ❌ `node_modules/` (já está no .gitignore)
- ❌ `dist/` (build de produção)
- ❌ `.env` (variáveis de ambiente)
- ❌ Logs e arquivos temporários

---

## 🔄 Atualizações Futuras

Sempre que fizer mudanças:

```bash
git add .
git commit -m "Descrição da mudança"
git push origin main
```

---

## 🎯 Deploy Automático na Vercel

Após subir no GitHub:

1. Acesse **vercel.com**
2. Clique em **"Add New Project"**
3. Importe o repositório `gstd-ag/crm-new`
4. Configure:
   - Framework Preset: **Vite**
   - Build Command: `npm run build`
   - Output Directory: `dist`
5. Clique em **Deploy**

**Pronto!** Seu site estará no ar em 2-3 minutos.

---

## 📊 Estrutura Final do Repositório

```
crm-new/
├── 📄 README.md                 # Documentação completa
├── 📱 SCRIPTS_WHATSAPP.md       # Scripts de vendas
├── 🚀 GUIA_IMPLANTACAO.md       # Guia de implantação
├── 📁 src/                      # Código fonte
│   ├── main.jsx
│   ├── index.css
│   └── components/
├── 📁 public/                   # Assets
├── 📦 package.json              # Dependências
├── ⚙️ vite.config.js            # Config Vite
├── 🎨 tailwind.config.js        # Config Tailwind
├── 🔍 eslint.config.js          # Linter
└── 🚫 .gitignore                # Ignorados
```

---

## 💡 Dicas

✅ **Commits frequentes:** Faça commits pequenos e descritivos  
✅ **Branch main:** Mantenha sempre funcional  
✅ **Tags de versão:** Use tags para releases (v1.0.0, v1.1.0)  
✅ **Changelog:** Atualize README com mudanças importantes  

---

**Boa sorte com o projeto! 🚀**

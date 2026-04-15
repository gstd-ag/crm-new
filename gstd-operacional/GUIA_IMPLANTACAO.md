# 🚀 GUIA DE IMPLANTAÇÃO - GSTD OPERACIONAL

> **Do zero ao primeiro cliente em 48 horas**

Este guia contém todos os passos para colocar o GSTD Operacional no ar e começar a vender sites ainda essa semana.

---

## 📋 CHECKLIST PRÉ-IMPLANTAÇÃO

### Antes de Começar
- [ ] Node.js 18+ instalado (`node -v`)
- [ ] Git instalado (`git --version`)
- [ ] Conta GitHub criada
- [ ] Conta Vercel criada (grátis)
- [ ] Extensão "Instant Data Scraper" instalada no Chrome
- [ ] WhatsApp Web acessível

---

## 🔧 PASSO 1: CLONAR E CONFIGURAR (30 min)

### 1.1 Clone o Repositório
```bash
git clone https://github.com/gstd-ag/crm-new.git
cd crm-new
```

### 1.2 Instale Dependências
```bash
npm install
```

### 1.3 Rode em Desenvolvimento
```bash
npm run dev
```

### 1.4 Acesse no Navegador
```
http://localhost:5173
```

✅ **Check:** Sistema rodando localmente?

---

## 🎨 PASSO 2: PERSONALIZAÇÃO INICIAL (15 min)

### 2.1 Configure Suas Metas
1. Vá em **Settings** ⚙️
2. Defina metas iniciais:
   - Diário: 20 leads
   - Semanal: 50 leads
   - Mensal: 200 leads
3. Salve

### 2.2 Meta Financeira do Mês
1. Em **Financeiro**
2. Ajuste meta para R$2000 (ou seu objetivo)
3. Ative/desative toggle de imposto (15,5%)

### 2.3 Teste Importação
1. Vá em **Importar Leads**
2. Cole um CSV de teste (use exemplo abaixo)
3. Clique em **Processar**
4. Verifique se lead apareceu no CRM

**CSV de Teste:**
```csv
link,nome,nota,avaliacao,nicho,endereco,funcionamento,site,telefone
https://google.com/maps/place/Teste,Restaurante Sabor,4.5,(120),Restaurante,Rua 123,Aberto,www.teste.com.br,(61) 99999-9999
```

✅ **Check:** Lead importado com preço correto?

---

## 📊 PASSO 3: CAPTAÇÃO DE LEADS REAIS (2 horas)

### 3.1 Escolha Nicho e Região
**Sugestões Iniciais:**
- Restaurantes em Taguatinga
- Clínicas em Águas Claras
- Mecânicas em Ceilândia
- Salões em Samambaia

### 3.2 Use Google Maps + Instant Data Scraper

**Passo a Passo:**
1. Abra Google Maps
2. Pesquise: `"restaurantes em Taguatinga"`
3. Role a página para carregar 20-30 resultados
4. Clique na extensão **Instant Data Scraper**
5. Aguarde extração automática
6. Clique em **Download CSV**

### 3.3 Limpeza do CSV (5 min)
1. Abra CSV no Excel/Google Sheets
2. Remova linhas em branco
3. Remova entries patrocinados
4. Verifique se colunas estão corretas:
   - `nome` ✅
   - `telefone` ou coluna com telefone ✅
   - `endereco` ✅
   - `nota` ✅
   - `site` (se tiver) ✅

### 3.4 Importe no GSTD Operacional
1. Copie todo conteúdo do CSV (Ctrl+A, Ctrl+C)
2. No sistema: **Importar Leads**
3. Cole no textarea gigante
4. Clique **Processar**
5. Confirme quantidade de leads

✅ **Check:** 20+ leads na coluna "Captado"?

---

## 💬 PASSO 4: ABORDAGEM VIA WHATSAPP (1 hora)

### 4.1 Prepare Scripts
1. Tenha o arquivo `SCRIPTS_WHATSAPP.md` aberto
2. Identifique nicho de cada lead
3. Copie script correspondente

### 4.2 Envie Mensagens
1. No CRM, clique 📱 no primeiro lead
2. WhatsApp Web abre com número
3. Cole script personalizado:
   - Substitua `[NOME]` pelo nome do contato
   - Substitua `[REGIÃO]` pela região
   - Substitua `[NOME DO NEGÓCIO]` pelo nome da empresa
4. Envie mensagem
5. Volte ao CRM e mova para **"WhatsApp Enviado"**

### 4.3 Repita para Todos
- Meta: 20 WhatsApps enviados
- Tempo estimado: 3 min por lead = 1 hora
- Faça em blocos de 10 com pausa

✅ **Check:** 20 leads em "WhatsApp Enviado"?

---

## 🏗️ PASSO 5: CRIAÇÃO DE SITES COM IA (2-3 horas)

### 5.1 Lead Respondeu com Interesse?
Quando cliente responder "sim", "quero ver", "me manda":

1. Mova lead para **"Preview Pronto"**
2. Clique 📋 **Copiar PRD**
3. PRD vai para clipboard automaticamente

### 5.2 Gere Site com IA

**Opção A: Cursor (Recomendado)**
```bash
# Se já tem Cursor instalado
1. Abra Cursor
2. Crie novo projeto React + Vite
3. Ctrl+K → Cole PRD
4. Aguarde IA gerar código (15-30 min)
5. npm run dev → Veja resultado
```

**Opção B: v0.dev (Online)**
```
1. Acesse v0.dev
2. Cole PRD no chat
3. IA gera site instantaneamente
4. Exporte código
```

**Opção C: Claude/ChatGPT + Replit**
```
1. Cole PRD no Claude/ChatGPT
2. Peça código completo React/Tailwind
3. Copie código
4. Cole no Replit.com
5. Execute e publique
```

### 5.3 Publique Preview
**Hostinger (Recomendado):**
```
1. Acesse Hostinger Business
2. Crie subdomínio: gstd.com.br/[cliente]
3. Upload dos arquivos do site
4. Teste link no celular
5. Copie URL
```

**Vercel (Alternativa Grátis):**
```bash
1. npm run build
2. vercel --prod
3. Gere link temporário
```

### 5.4 Envie Preview pro Cliente
```
Olá [NOME]! 👍

Seu preview tá no ar: 
👉 [LINK DO SITE]

Dá uma olhada no celular e me diz o que achou!
Qualquer ajuste é só falar.

Abs,
[SEU NOME]
```

✅ **Check:** Preview enviado em até 24h?

---

## 💰 PASSO 6: FECHAMENTO E COBRANÇA (30 min)

### 6.1 Cliente Aprovou?
Mova lead para **"Fechado"** no CRM

### 6.2 Configure Valores
1. Clique ✏️ **Editar** no card
2. Marque checkbox **Domínio Próprio** (+R$60)
3. Selecione upsells:
   - [ ] Manutenção Básica R$67/mês
   - [ ] Manutenção Premium R$97/mês
   - [ ] GMN R$97/mês
4. Preencha campos:
   - **Previsto:** Valor total
   - **Realizado:** Entrada recebida (50%)

### 6.3 Envie Proposta Formal
```
[NOME], bora formalizar? 🎉

PROPOSTA:
✅ Site Profissional Mobile-First
✅ Hospedagem Incluída (1 ano)
✅ Botão WhatsApp
✅ SEO Otimizado
✅ Domínio: [dominiocliente.com.br]

INVESTIMENTO:
Site: R$ [VALOR]
Domínio: R$ 60
Total: R$ [TOTAL]

FORMA DE PAGAMENTO:
- 50% entrada: R$ [METADE] (Pix)
- 50% entrega: R$ [METADE] (7 dias)

MANUTENÇÃO OPCIONAL:
R$ 67/mês (atualizações, backups, suporte)

PIX:
Chave: [SUA CHAVE]
Nome: [SEU NOME]

Bora começar? Me avisa quando fizer o Pix!
```

### 6.4 Receba e Comece Produção
1. Confirme pagamento no CRM
2. Atualize campo **Realizado**
3. Inicie produção do site final
4. Entregue em 48-72h

✅ **Check:** Primeiro pagamento recebido?

---

## 📈 PASSO 7: ROTINA DIÁRIA DE SUCESSO

### Manhã (08:00 - 10:00)
- [ ] Abrir Google Maps
- [ ] Extrair 20 novos leads
- [ ] Importar no CRM
- [ ] Enviar 10 WhatsApps

### Tarde (14:00 - 17:00)
- [ ] Responder clientes interessados
- [ ] Gerar PRDs
- [ ] Criar sites com IA
- [ ] Enviar previews

### Fim de Tarde (17:00 - 18:00)
- [ ] Follow-up D+2, D+5, D+10
- [ ] Fechar vendas
- [ ] Registrar pagamentos

### Noite (18:00 - 18:30)
- [ ] Abrir **Dashboard**
- [ ] Verificar metas do dia
- [ ] Abrir **Financeiro**
- [ ] Conferir previsto vs realizado
- [ ] Planejar próximo dia

---

## 🎯 METAS PROGRESSIVAS

### Semana 1 (Aprendizado)
- [ ] 100 leads capturados
- [ ] 50 WhatsApps enviados
- [ ] 10 previews gerados
- [ ] **3 clientes fechados**
- [ ] R$900-1500 faturados

### Semana 2 (Otimização)
- [ ] 150 leads capturados
- [ ] 75 WhatsApps enviados
- [ ] Refinar scripts
- [ ] **5 clientes fechados**
- [ ] R$1500-2500 faturados
- [ ] Ativar primeiras recorrências

### Mês 1 (Consolidação)
- [ ] 600 leads totais
- [ ] 300 contatados
- [ ] **15 clientes fechados**
- [ ] R$4500-7500 faturados
- [ ] R$1000+ MRR (recorrência)

### Mês 2 (Escala)
- [ ] 1200 leads totais
- [ ] 600 contatados
- [ ] **30 clientes fechados**
- [ ] R$9000-15000 faturados
- [ ] R$2000+ MRR
- [ ] Considerar equipe de vendas

---

## 🛠️ FERRAMENTAS ESSENCIAIS

### Gratuitas
| Ferramenta | Uso | Link |
|-----------|-----|------|
| **Cursor** | IDE com IA | cursor.com |
| **Instant Data Scraper** | Extrair Google Maps | Chrome Web Store |
| **Vercel** | Deploy grátis | vercel.com |
| **Google AI Studio** | IA pra gerar sites | aistudio.google.com |
| **WhatsApp Web** | Envio em massa | web.whatsapp.com |

### Pagas (Opcionais)
| Ferramenta | Custo | Benefício |
|-----------|-------|-----------|
| **Hostinger Business** | R$30/mês | Domínios ilimitados |
| **Claude Pro** | $20/mês | IA mais potente |
| **Canva Pro** | R$50/mês | Artes para redes |

---

## 🚨 SOLUÇÃO DE PROBLEMAS

### "Leads não estão sendo importados"
✅ Verifique se CSV tem cabeçalho  
✅ Confira se colunas têm nomes corretos  
✅ Remova linhas vazias  

### "Precificação não funciona"
✅ Regiões devem ser escritas exatamente como no código  
✅ Verifique maiúsculas/minúsculas  
✅ Regiões não mapeadas = R$297 (padrão)  

### "WhatsApp não abre"
✅ Número deve ter DDD e 9 dígitos  
✅ Formato: 5561999999999 (sem traços/espaços)  
✅ Use Chrome/Edge  

### "IA não gera site bom"
✅ Melhore o PRD com mais detalhes  
✅ Especifique cores, seções, tom de voz  
✅ Use Cursor em vez de ChatGPT gratuito  

### "Cliente não responde WhatsApp"
✅ Espere 48h antes do follow-up  
✅ Personalize mais a mensagem  
✅ Ofereça algo de valor (dica, insight)  

---

## 📞 SUPORTE E COMUNIDADE

### Dúvidas Técnicas
- GitHub Issues: https://github.com/gstd-ag/crm-new/issues
- Documentação: README.md no repositório

### Dúvidas de Vendas
- Scripts: SCRIPTS_WHATSAPP.md
- Objeções: Veja respostas prontas no guia

### Evolução do Sistema
- Fase 2: Integração Supabase
- Fase 3: API Google Places
- Fase 4: Automação de follow-up

---

## 🎁 BÔNUS: TEMPLATES PRONTOS

### Template de Proposta (PDF)
Use Canva para criar template profissional com:
- Logo da sua agência
- Descrição do serviço
- Investimento
- Formas de pagamento
- Seu contato

### Template de Contrato
Modelo simples de prestação de serviços:
- Escopo do projeto
- Prazos de entrega
- Valores e condições
- Direitos autorais
- Assinatura digital

### Template de Onboarding
Quando cliente fechar, envie:
```
🎉 Bem-vindo!

Prazer trabalhar com você!

Próximos passos:
1. Me envie logo/cores (se tiver)
2. Texto sobre sua empresa
3. Fotos do negócio (opcional)
4. Aprovação em até 48h

Entrega: [DATA]
Dúvidas: Tô aqui!

Vamos juntos! 🚀
```

---

> 🚀 **Hora de agir!**  
> Siga este guia passo a passo e em 48h você está com o sistema rodando e os primeiros leads sendo contatados.  
> **O segredo é: Ação massiva → Ajuste rápido → Escala consistente.**

**Boa venda e sucesso! 🎯💰**

# 🔧 **CONFIGURAÇÕES PARA ATUALIZAR - ADHAMOS**

## ⚠️ **ATENÇÃO: SUBSTITUA ESTES DADOS ANTES DE COLOCAR NO AR!**

---

## 📱 **1. WHATSAPP**

### **Número atual (placeholder):** 
```
5511XXXXXXXXX
```

### **🔄 Trocar em 3 lugares:**

#### **1.1 index.html - Linha ~710 (CTA Final)**
```html
<!-- ANTES -->
<a href="https://wa.me/5511XXXXXXXXX?text=Olá,%20quero%20saber%20mais...">

<!-- DEPOIS (exemplo) -->
<a href="https://wa.me/5511987654321?text=Olá,%20quero%20saber%20mais...">
```

#### **1.2 index.html - Footer (Linha ~756)**
```html
<!-- ANTES -->
<p><i class="fab fa-whatsapp"></i> (11) 9XXXX-XXXX</p>

<!-- DEPOIS -->
<p><i class="fab fa-whatsapp"></i> (11) 98765-4321</p>
```

#### **1.3 js/main.js - Redirecionamento (Linha ~48)**
```javascript
// ANTES
window.location.href = `https://wa.me/5511999999999?text=${whatsappMsg}`;

// DEPOIS
window.location.href = `https://wa.me/5511987654321?text=${whatsappMsg}`;
```

### **✅ Formato correto:**
- Internacional: `55` (Brasil) + `11` (DDD) + `987654321` (número com 9 dígitos)
- Exemplo completo: `5511987654321`
- **SEM espaços, traços ou parênteses!**

---

## 📧 **2. E-MAILS**

### **E-mails para atualizar:**

#### **2.1 E-mail de Contato Geral**
```
📧 Atual: contato@adhamos.com.br
📍 Onde está: index.html (footer), politica-privacidade.html, termos-uso.html
```

#### **2.2 E-mail de Privacidade (DPO)**
```
📧 Atual: privacidade@adhamos.com.br
📍 Onde está: politica-privacidade.html (seção 7 e 11)
```

#### **2.3 Google Apps Script - Notificações**
```javascript
// google-apps-script.gs - Linha 34
const emailDestino = 'contato@adhamos.com.br'; // TROCAR AQUI
```

---

## 📞 **3. TELEFONE FIXO**

### **Atualizar em:**

#### **3.1 Footer (index.html)**
```html
<!-- ANTES -->
<p><i class="fas fa-phone"></i> (11) XXXXX-XXXX</p>

<!-- DEPOIS -->
<p><i class="fas fa-phone"></i> (11) 3XXX-XXXX</p>
```

#### **3.2 Política de Privacidade**
```html
<!-- politica-privacidade.html - Seção 11 -->
<p><strong>📱 Telefone:</strong> (11) 3XXX-XXXX</p>
```

#### **3.3 Termos de Uso**
```html
<!-- termos-uso.html - Seção 11 -->
<p><strong>📱 WhatsApp:</strong> (11) 9XXXX-XXXX</p>
```

---

## 🏢 **4. ENDEREÇO DA EMPRESA**

### **Atualizar endereço completo em:**

#### **4.1 Footer (index.html)**
```html
<!-- ANTES -->
<p><i class="fas fa-map-marker-alt"></i> São Paulo, SP</p>

<!-- DEPOIS (exemplo) -->
<p><i class="fas fa-map-marker-alt"></i> Rua Exemplo, 123 - Bairro - São Paulo/SP - CEP 01234-567</p>
```

#### **4.2 Política de Privacidade (Seção 11)**
```html
<p><strong>📍 Endereço:</strong> [Endereço Completo da Adhamos]</p>
```

#### **4.3 Termos de Uso (Seção 11)**
```html
<p><strong>📍 Endereço:</strong> [Endereço Completo da Adhamos]</p>
```

---

## 🏛️ **5. CNPJ**

### **Adicionar em:**

#### **5.1 Footer (index.html) - Já tem placeholder**
```html
<p style="margin-top: 1rem; font-size: 0.875rem;">CNPJ: XX.XXX.XXX/XXXX-XX</p>
```

**Trocar por:** `CNPJ: 12.345.678/0001-90` (exemplo)

---

## 🔗 **6. REDES SOCIAIS**

### **Links para atualizar no Footer:**

#### **6.1 LinkedIn**
```html
<!-- ANTES -->
<a href="https://linkedin.com/company/adhamos" target="_blank">

<!-- DEPOIS -->
<a href="https://linkedin.com/company/SEU_PERFIL" target="_blank">
```

#### **6.2 Instagram**
```html
<!-- ANTES -->
<a href="https://instagram.com/adhamos" target="_blank">

<!-- DEPOIS -->
<a href="https://instagram.com/SEU_PERFIL" target="_blank">
```

#### **6.3 Facebook**
```html
<!-- ANTES -->
<a href="https://facebook.com/adhamos" target="_blank">

<!-- DEPOIS -->
<a href="https://facebook.com/SUA_PAGINA" target="_blank">
```

---

## 📊 **7. GOOGLE TAG MANAGER**

### **Configurar no index.html (head):**

#### **Passo 1: Criar conta GTM**
1. Acesse: https://tagmanager.google.com
2. Crie nova conta: "Adhamos"
3. Container: "Landing Page NR-1"
4. Plataforma: Web
5. Copie o ID (formato: GTM-XXXXXXX)

#### **Passo 2: Colar no código**
```html
<!-- index.html - Linha 9 -->
<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
})(window,document,'script','dataLayer','GTM-XXXXXXX');</script>
                                            ^^^^^^^^^^^ TROCAR AQUI
```

E também no `<body>`:
```html
<!-- index.html - Linha 32 -->
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-XXXXXXX"
                                                                  ^^^^^^^^^^^ TROCAR AQUI
```

---

## 📈 **8. FACEBOOK PIXEL**

### **Configurar no index.html (head):**

#### **Passo 1: Obter Pixel ID**
1. Acesse: https://business.facebook.com
2. Configurações de Eventos > Pixels
3. Copie o Pixel ID (números apenas)

#### **Passo 2: Colar no código**
```html
<!-- index.html - Linha 18 -->
fbq('init', 'YOUR_PIXEL_ID');
            ^^^^^^^^^^^^^^^ TROCAR pelo seu Pixel ID (ex: 1234567890123456)
```

E na tag noscript:
```html
<!-- index.html - Linha 27 -->
<img height="1" width="1" src="https://www.facebook.com/tr?id=YOUR_PIXEL_ID&ev=PageView&noscript=1"/>
                                                              ^^^^^^^^^^^^^^^ TROCAR
```

---

## 📊 **9. GOOGLE SHEETS (Captação de Leads)**

### **Configurar integração:**

#### **Passo 1: Criar planilha**
1. Acesse: https://sheets.google.com
2. Crie: "Leads NR-1 - Adhamos"
3. Copie o ID da URL (entre `/d/` e `/edit`)

#### **Passo 2: Google Apps Script**
1. Acesse: https://script.google.com
2. Novo projeto
3. Cole o código de `google-apps-script.gs`
4. **Linha 10:** Cole o ID da planilha
   ```javascript
   const SHEET_ID = 'COLE_AQUI_O_ID_DA_SUA_PLANILHA';
   ```
5. **Linha 34:** Cole seu e-mail
   ```javascript
   const emailDestino = 'seuemail@adhamos.com.br';
   ```

#### **Passo 3: Deploy**
1. Deploy > Nova implantação
2. Tipo: Aplicativo Web
3. Execute as: "Eu"
4. Acesso: "Qualquer pessoa"
5. Deploy > Copie a URL

#### **Passo 4: Atualizar landing page**
```javascript
// integracao-google-sheets.js - Linha 15
const SCRIPT_URL = 'COLE_A_URL_DO_PASSO_3_AQUI';
```

Copie o conteúdo completo de `integracao-google-sheets.js` e cole no `js/main.js` (substitua a função do formulário, linha ~44)

---

## 🔐 **10. POLÍTICA DE PRIVACIDADE E TERMOS**

### **Arquivos criados:**
✅ `politica-privacidade.html` - Completa e conforme LGPD  
✅ `termos-uso.html` - Termos de uso do site  

### **O que AINDA precisa atualizar neles:**

1. **Endereço completo** (3 lugares)
2. **Telefones** (2 lugares cada)
3. **E-mail do DPO** (se diferente de privacidade@adhamos.com.br)

---

## ✅ **CHECKLIST FINAL DE CONFIGURAÇÃO**

Antes de colocar no ar, confirme:

### **Informações da Empresa:**
- [ ] WhatsApp atualizado (3 lugares)
- [ ] E-mail de contato atualizado (4 lugares)
- [ ] E-mail de privacidade atualizado (2 lugares)
- [ ] Telefone fixo atualizado (3 lugares)
- [ ] Endereço completo atualizado (4 lugares)
- [ ] CNPJ adicionado (1 lugar)
- [ ] Links de redes sociais atualizados (3 lugares)

### **Integrações:**
- [ ] Google Tag Manager configurado (2 lugares)
- [ ] Facebook Pixel configurado (2 lugares)
- [ ] Google Sheets + Apps Script configurado
- [ ] Webhook integrado (se usar Make.com ou RD Station)

### **Páginas Legais:**
- [ ] Política de Privacidade revisada e personalizada
- [ ] Termos de Uso revisados
- [ ] Links funcionando no footer

### **Testes:**
- [ ] Formulário envia corretamente
- [ ] WhatsApp abre com mensagem pré-preenchida
- [ ] E-mails de notificação chegam
- [ ] Google Sheets registra leads
- [ ] Todos os links estão funcionando
- [ ] Responsivo testado em mobile

---

## 🚀 **ORDEM RECOMENDADA DE CONFIGURAÇÃO:**

1. ✅ **Informações básicas** (10 min)
   - WhatsApp, e-mails, telefone, endereço, CNPJ

2. ✅ **Google Sheets** (15 min)
   - Criar planilha
   - Configurar Apps Script
   - Testar captura de lead

3. ✅ **Tracking** (10 min)
   - Google Tag Manager
   - Facebook Pixel

4. ✅ **Redes sociais** (5 min)
   - LinkedIn, Instagram, Facebook

5. ✅ **Testes finais** (10 min)
   - Testar tudo antes de subir

**Total: ~50 minutos** ⏱️

---

## 📞 **PRECISA DE AJUDA?**

Se tiver dúvida em qualquer configuração, me avise indicando:
- Qual item você está configurando
- Qual erro está aparecendo
- Print do problema (se possível)

Estou aqui para ajudar! 🚀
# Deploy no Vercel - Guia Rápido

## 📋 Pré-requisitos

1. Conta no GitHub
2. Conta no Vercel (gratuita)
3. Logo `digitalnest-logo.png` no diretório raiz

## 🚀 Passos para Deploy

### 1. Preparar o Repositório

Certifique-se de que você tem os seguintes arquivos:
- ✅ `index.html` (arquivo principal)
- ✅ `digitalnest-logo.png` (logo da DigitalNest)
- ✅ `vercel.json` (configuração do Vercel)
- ✅ `README.md` (documentação)
- ✅ `.gitignore` (arquivos a ignorar)

### 2. Subir para o GitHub

```bash
git add .
git commit -m "Preparar para deploy no Vercel"
git push origin main
```

### 3. Deploy no Vercel

#### Opção A: Via Interface Web (Recomendado)

1. Acesse [vercel.com](https://vercel.com)
2. Faça login com sua conta GitHub
3. Clique em "New Project"
4. Selecione o repositório `apresentacaomeujaboatao`
5. Configure:
   - **Framework Preset**: Other
   - **Root Directory**: `./`
   - **Build Command**: (deixe vazio)
   - **Output Directory**: (deixe vazio)
6. Clique em "Deploy"

#### Opção B: Via CLI

```bash
# Instalar Vercel CLI
npm install -g vercel

# Fazer login
vercel login

# Deploy
vercel
```

### 4. Verificar o Deploy

Após o deploy, o Vercel fornecerá uma URL como:
```
https://meu-jaboatao-apresentacao.vercel.app
```

## 📝 Notas Importantes

### Logo DigitalNest
- A logo está configurada com caminho relativo `./digitalnest-logo.png`
- Se a logo não carregar, ela será ocultada automaticamente (fallback)
- Certifique-se de que o arquivo `digitalnest-logo.png` está no repositório

### Domínio Customizado (Opcional)
Para usar um domínio próprio:
1. No dashboard do Vercel, vá em "Settings"
2. Clique em "Domains"
3. Adicione seu domínio customizado

## 🔄 Atualizações Automáticas

Qualquer commit na branch `main` dispara um novo deploy automaticamente!

```bash
git add .
git commit -m "Atualizar apresentação"
git push origin main
```

## 🛠️ Troubleshooting

### Logo não aparece
1. Verifique se o arquivo existe no repositório
2. Confirme o nome: `digitalnest-logo.png` (minúsculas)
3. Limpe o cache do Vercel e faça redeploy

### Página em branco
1. Abra o console do navegador (F12)
2. Verifique erros no console
3. Confirme que `index.html` está na raiz

## 📞 Suporte

Em caso de dúvidas:
- 📧 contato@digitalnest.app.br
- 🌐 www.digitalnest.app.br

---

**Desenvolvido por DigitalNest** 💚

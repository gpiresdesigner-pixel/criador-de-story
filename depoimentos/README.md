# Plataforma de Depoimentos — Desafio -5kg em 7 Dias 💚

Plataforma simples para coletar depoimentos de alunas do desafio da Carol Zonato.  
Funciona 100% no navegador, sem necessidade de servidor ou banco de dados.

---

## Arquivos

| Arquivo | Descrição |
|---|---|
| `index.html` | Formulário público — link para as alunas |
| `admin.html` | Painel administrativo — apenas para Carol |
| `style.css` | Estilos (não precisa editar) |

---

## Como hospedar no GitHub Pages

### Passo 1 — Crie uma conta no GitHub
Acesse [github.com](https://github.com) e crie uma conta gratuita (se ainda não tiver).

### Passo 2 — Crie um repositório
1. Clique no botão verde **"New"** (ou **"Novo"**)
2. Dê um nome ao repositório, ex: `depoimentos-desafio`
3. Deixe como **Public** (público)
4. Clique em **"Create repository"**

### Passo 3 — Faça upload dos arquivos
1. Na página do repositório, clique em **"uploading an existing file"**
2. Arraste os três arquivos: `index.html`, `admin.html` e `style.css`
3. Clique em **"Commit changes"**

### Passo 4 — Ative o GitHub Pages
1. Vá em **Settings** (configurações do repositório)
2. No menu lateral, clique em **"Pages"**
3. Em **"Source"**, selecione **"Deploy from a branch"**
4. Em **"Branch"**, selecione **main** e clique **Save**
5. Aguarde 1-2 minutos

### Passo 5 — Pronto!
Seu link será algo como:
```
https://SEU-USUARIO.github.io/depoimentos-desafio/
```

Compartilhe esse link com as alunas! Para acessar o painel admin:
```
https://SEU-USUARIO.github.io/depoimentos-desafio/admin.html
```

---

## Senha do painel admin

A senha padrão é: **`carol2024`**

Para trocar a senha, abra o arquivo `admin.html` em um editor de texto,  
procure pela linha:
```
const SENHA_CORRETA = 'carol2024';
```
E substitua `carol2024` pela senha que preferir.

---

## Como exportar os depoimentos

1. Acesse o painel admin (`admin.html`)
2. Digite a senha
3. Clique no botão **"📥 Exportar CSV"**
4. Um arquivo `.csv` será baixado automaticamente
5. Abra no Excel ou Google Planilhas

---

## Onde ficam os dados?

Os depoimentos ficam salvos no **localStorage** do navegador de quem acessou o formulário.  
Isso significa que **os dados ficam no dispositivo da aluna** — não há servidor.

> **Dica importante:** Para centralizar os dados, instrua as alunas a preencher o formulário  
> sempre no mesmo dispositivo/navegador em que você irá visualizar o painel admin —  
> ou considere usar um serviço gratuito de backend (como Firebase ou Supabase) para uma versão mais avançada.

---

## Perguntas frequentes

**Os dados somem se a aluna fechar o navegador?**  
Não! O localStorage persiste mesmo após fechar e reabrir o navegador.

**Funciona no celular?**  
Sim! O formulário foi criado pensando em uso mobile.

**Posso usar sem internet?**  
Sim, basta abrir o arquivo `index.html` diretamente no navegador.

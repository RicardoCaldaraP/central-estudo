# 📖 Central de Estudo Mozão

Plataforma de estudos com atividades em JSON, hospedada no GitHub Pages.

---

## 🚀 Como publicar no GitHub (passo a passo)

### Passo 1 — Criar uma conta no GitHub
Acesse https://github.com e crie uma conta gratuita se ainda não tiver.

---

### Passo 2 — Criar o repositório
1. Clique no botão **"New"** (canto superior esquerdo)
2. Em **Repository name**, coloque: `central-estudo`
3. Selecione **Public**
4. Marque **"Add a README file"**
5. Clique em **"Create repository"**

---

### Passo 3 — Fazer upload dos arquivos do site
1. Dentro do repositório, clique em **"Add file" → "Upload files"**
2. Arraste o arquivo `index.html`
3. Clique em **"Commit changes"**

---

### Passo 4 — Criar a pasta de atividades e subir os JSONs
1. Clique em **"Add file" → "Create new file"**
2. No campo de nome, digite: `atividades/ebusiness-parte1.json`
3. Cole o conteúdo do arquivo `ebusiness-parte1.json`
4. Clique em **"Commit changes"**
5. Repita para o `ebusiness-parte2.json`

---

### Passo 5 — Ativar o GitHub Pages
1. No repositório, clique em **"Settings"** (aba no topo)
2. No menu lateral, clique em **"Pages"**
3. Em **"Source"**, selecione: `Deploy from a branch`
4. Em **"Branch"**, selecione: `main` e pasta `/ (root)`
5. Clique em **"Save"**
6. Aguarde 1-2 minutos

Seu site estará disponível em:
`https://SEU_USUARIO.github.io/central-estudo`

---

### Passo 6 — Gerar o Token de Acesso (para upload pelo site)
O token permite que o site faça upload de novos JSONs direto para o GitHub.

1. Acesse: https://github.com/settings/tokens
2. Clique em **"Generate new token (classic)"**
3. Em **"Note"**, coloque: `central-estudo`
4. Em **"Expiration"**, selecione **"No expiration"**
5. Marque a caixinha **"repo"** (a primeira da lista)
6. Clique em **"Generate token"** no final da página
7. **COPIE O TOKEN AGORA** (ele só aparece uma vez!)
   - Ele começa com `ghp_`

---

### Passo 7 — Configurar o site
1. Acesse seu site no GitHub Pages
2. Clique no botão **"⚙️ Config"** no canto superior direito
3. Preencha:
   - **Usuário do GitHub**: seu nome de usuário
   - **Nome do repositório**: `central-estudo`
   - **Token**: cole o token que você copiou
4. Clique em **"Salvar"**
5. Pronto! As atividades vão aparecer automaticamente.

---

## 📱 Acessar de outros dispositivos
Basta acessar o mesmo link do GitHub Pages em qualquer dispositivo.
O token fica salvo no navegador de cada dispositivo — configure uma vez por aparelho.

---

## 📤 Adicionar novas atividades
Você tem duas opções:

**Pelo site** (mais fácil):
- Clique em "Importar Atividades"
- Selecione o arquivo .json
- Clique em "Importar"

**Pelo GitHub** (alternativa):
- Acesse o repositório
- Vá na pasta `atividades/`
- Clique em "Add file" → "Upload files"
- Faça upload do .json

---

## 📋 Padrão de JSON para novas atividades

```json
{
  "id": "identificador-unico",
  "titulo": "Título do Conjunto",
  "descricao": "Descrição do conteúdo.",
  "disciplina": "Nome da Disciplina",
  "criado_em": "YYYY-MM-DD",
  "cor": "#HEX",
  "icone": "📚",
  "questoes": [
    {
      "id": "q001",
      "tipo": "multipla_escolha",
      "enunciado": "Pergunta aqui?",
      "opcoes": ["Opção A", "Opção B", "Opção C", "Opção D"],
      "resposta": "Opção correta",
      "explicacao": "Por que esta é a resposta certa."
    },
    {
      "id": "q002",
      "tipo": "verdadeiro_falso",
      "enunciado": "Afirmação aqui.",
      "resposta": true,
      "explicacao": "Explicação."
    },
    {
      "id": "q003",
      "tipo": "ligar_colunas",
      "enunciado": "Ligue os itens:",
      "pares": [
        { "esquerda": "Item A", "direita": "Correspondente A" },
        { "esquerda": "Item B", "direita": "Correspondente B" }
      ],
      "explicacao": "Explicação das correspondências."
    }
  ]
}
```

---

Feito com 💜 por mozin

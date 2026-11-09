# Passo a passo — criar o repositório e publicar a release

Faça tudo pelo site do GitHub, no navegador. Dura uns 3 minutos.

## 1. Criar o repositório

1. Abra <https://github.com/new>.
2. **Repository name:** `legas-keys-downloads` (ou outro nome curto).
3. **Description:** `Downloads do Legas Keys Desktop`.
4. **Public** (precisa ser público para o asset da release ser baixável sem login).
5. Marque **Add a README file**.
6. Clique em **Create repository**.

## 2. Subir o README deste pacote (opcional, substitui o README padrão)

1. No repositório recém-criado, clique em `README.md` → ícone de lápis (Edit).
2. Apague o conteúdo.
3. Cole o conteúdo de `README.md` que está nesta pasta.
4. Rolar até o rodapé → **Commit changes**.

## 3. Criar a release com o .exe

1. No repositório, aba **Releases** (na lateral direita, ou URL `.../releases`).
2. Clique em **Draft a new release** (ou **Create a new release** da primeira vez).
3. **Choose a tag:** digite `v0.6.24` e clique em `Create new tag: v0.6.24 on publish`.
4. **Release title:** `Legas Keys 0.6.24`.
5. **Describe this release:**
   ```
   Fallback multi-fornecedor quando o Ryuu falha:
   - SteamAutoCracks/ManifestHub
   - steamtools-games/ManifestHub3
   - trionine/ManifestHub
   - SteamTools-Team/GameList
   Zip das branches é lido, key.vdf é convertida em .lua automaticamente.
   ```
6. Em **Attach binaries by dropping them here or selecting them**: arraste
   `Legas-Keys-0.6.24.exe` desta pasta.
7. Espere o upload terminar (35 MB, barra de progresso aparece).
8. Clique em **Publish release**.

## 4. Pegar a URL direta do .exe

1. Na página da release publicada, role até **Assets**.
2. Clique com o botão direito em `Legas-Keys-0.6.24.exe` → **Copiar endereço do link**.
3. O link vai estar nesse formato:
   `https://github.com/{seu-usuario}/legas-keys-downloads/releases/download/v0.6.24/Legas-Keys-0.6.24.exe`

## 5. Me mandar o link

Cola o link aqui que eu atualizo o `repo/lib/legas-release.ts` com a nova
versão e URL. Depois é só redeployar o site e os clientes já baixam pelo
GitHub em vez do Supabase.

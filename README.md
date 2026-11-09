# Legas Keys — Downloads

Repositório usado só para hospedar o executável do Legas Keys Desktop como
GitHub Release, fora do Supabase Storage (que estava sangrando o egress da
Free). GitHub Releases têm egress ilimitado e não contam para nenhuma cota.

## Último build

- **Legas Keys 0.6.24** — [baixar](../../releases/latest)

## Como atualizar

1. Compilar o novo `Legas-Keys-X.Y.Z.exe`.
2. Abrir `Releases → Draft a new release`.
3. Criar a tag `vX.Y.Z` a partir de `main`.
4. Anexar o `.exe` como asset.
5. Publicar.
6. Atualizar `NEXT_PUBLIC_LEGAS_APP_URL` e `NEXT_PUBLIC_LEGAS_APP_VERSION`
   no site (ou o fallback em `repo/lib/legas-release.ts`) para apontar para
   a URL do novo asset.

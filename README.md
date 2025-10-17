# ResolvePrev – Next.js + Tailwind

Projeto pronto para deploy na Vercel (App Router).

## Rodar localmente
```bash
npm install
npm run dev
# http://localhost:3000
```

## Subir no GitHub (2 opções)

### A) CLI do GitHub (recomendado)
```bash
# dentro da pasta do projeto
gh repo create resolveprev-site --public --source . --remote origin --push
```

### B) Git padrão
```bash
git init
git add .
git commit -m "ResolvePrev: primeira versão"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/resolveprev-site.git
git push -u origin main
```

## Deploy na Vercel
1. Importe o repositório na Vercel (Add New → Project).
2. A detecção de Next.js é automática. Mantenha:
   - Build: `next build`
   - Output: `.next`
3. Deploy!
4. (Opcional) Adicione seu domínio em *Settings → Domains*.

---

O seu componente está em `src/components/ResolvePrevLanding.tsx`.
A página principal (`src/app/page.tsx`) simplesmente o renderiza.
Se usar imagens remotas (ex.: i.ibb.co), já há permissão em `next.config.mjs`.

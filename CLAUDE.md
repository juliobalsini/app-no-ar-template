# Projeto: <nome>
<uma frase: o que o app faz e para quem>

## Stack
- Next.js (App Router) + TypeScript + Tailwind
- Supabase (Postgres, Auth, Storage) via @supabase/ssr
- Deploy: Vercel (push na main = produção)

## Comandos
- Dev: `npm run dev` · Build: `npm run build` · Lint: `npm run lint`
- Migration: `npx supabase migration new <nome>` → `npx supabase db push`
- Tipos: `npx supabase gen types typescript --linked > lib/database.types.ts`

## Regras
- Responda e comente em português.
- Banco só muda por migration; toda tabela nova com RLS e política.
- Chave secreta só em código de servidor; nunca com prefixo NEXT_PUBLIC_.
- Nunca commitar arquivos .env.
- Commit só com `npm run build` passando; mensagens curtas no imperativo.
- Tarefa ambígua: pergunte antes de executar.

## Pronto quando
- Build passa sem erro de tipo.
- Funciona no preview da Vercel.
- Regra nova aprendida foi acrescentada aqui.

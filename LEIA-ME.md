# Site Foto no Clássico — como publicar na Vercel

## 1. Antes de subir (2 ajustes obrigatórios)
No final do `index.html`, no bloco CONFIGURAÇÃO:
- `WHATSAPP` → seu número com DDI+DDD, só dígitos (ex.: 5511999998888)
- `INSTAGRAM` → já está @fotonoclassico; troque se for outro

## 2. Fotos (pasta /img) — já preenchida com as fotos reais; para trocar, mantenha os nomes
Coloque as fotos com estes nomes (JPG, ~1600px de largura, até ~300 KB cada):
| Arquivo | Onde aparece | Sugestão |
|---|---|---|
| hero.jpg | Fundo do topo | Kombi com neon à noite (horizontal) |
| kombi.jpg | Card Kombi | Kombi montada |
| fusca.jpg | Card Fusca | Fusca azul faróis acesos |
| telefone.jpg / telefone-2.jpg | Audio guestbook | Telefone retrô / convidado gravando (vertical) |
| neon.jpg | Ambientação | Neon + malas de época |
| aderecos.jpg | Adereços | Amigos com adereços |
| galeria-1 a galeria-7.jpg | Galeria | Momentos reais (1 e 5 verticais; 2 e 6 horizontais) |
| og.jpg | Prévia no WhatsApp/Facebook | 1200x630 |

Se alguma foto faltar, o site mostra um fundo elegante no lugar — nada quebra.

## 3. Publicar
1. vercel.com → Add New → Project → arraste esta pasta (ou suba num repositório GitHub e importe).
2. Framework Preset: **Other**. Sem build command. Deploy.
3. Settings → Domains → adicione `fotonoclassico.agenciamaiscriativa.com.br`.
4. No DNS do agenciamaiscriativa.com.br crie: **CNAME** · nome `fotonoclassico` · valor `cname.vercel-dns.com`.
   (A Vercel confirma o valor exato na tela de Domains.) SSL é automático.

## 4. Opcional — medir conversões
O formulário já dispara `generate_lead` (Google Analytics/gtag) e `Lead` (Meta Pixel) se você colar esses scripts no `<head>`.

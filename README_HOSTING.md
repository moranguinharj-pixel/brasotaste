Guia de Hospedagem & Deploy — Braso Taste

Recomendado: Vercel (suporta Next.js automaticamente)

1) Criar repositório no GitHub e fazer push de todo o conteúdo deste diretório.
2) No Vercel: New Project -> Import Git Repository -> Deploy.
3) Substitua imagens em /public por assets finais (hero, og, gallery, logo).
4) Em Vercel, adicione domínio customizado e aponte DNS (CNAME/A) conforme instruções do provedor de domínio.
5) Para Netlify: conecte repositório; build command: npm run build ; publish directory: .next
6) Em servidor próprio: npm install; npm run build; npm run start (use PM2/systemd); configure Nginx como proxy e Let's Encrypt para SSL.

SEO e Indexação
- Use o arquivo /public/sitemap.xml para enviar ao Google Search Console.
- Substitua /public/og.jpg por imagem 1200x630px para redes sociais.
- Opcional: incluir GA4 ou Tag Manager no _document.js para analytics.

Quer que eu faça o deploy no Vercel para você (preciso de acesso ao GitHub ou permissão para criar o repositório)?
# robots.txt Configuration

This `robots.txt` file defines which user-agents (bots) are allowed or disallowed to access specific sections of the website. It helps in controlling how search engines and other automated systems crawl and index the website content.

## Contents of robots.txt

```plaintext
User-agent: *
Allow: /
Disallow: /finalizacao/carrinho
Disallow: /account*
Disallow: /*/?map=productClusterIds

User-agent: Googlebot
Allow: /
Disallow: /finalizacao/carrinho
Disallow: /account*
Disallow: /*/?map=productClusterIds

User-agent: AdsBot-Google
Allow: /
Disallow: /finalizacao/carrinho
Disallow: /account*
Disallow: /*/?map=productClusterIds

User-agent: Screaming Frog SEO Spider
Allow: /

User-agent: EtaoSpider
Disallow: /

User-agent: GPTBot
Disallow: /

User-agent: CCBot
Disallow: /

Sitemap: https://www.bemol.com.br/sitemap.xml

```

Explanation of Rules
User-agent: *
Applies to all bots. All pages are allowed, except:

/finalizacao/carrinho: Cart checkout is disallowed.
/account*: Any page related to user accounts is disallowed.
/*/?map=productClusterIds: Specific product cluster URLs are disallowed.
User-agent: Googlebot
Applies specifically to Googlebot. Same rules as above, with the same disallowed paths.

User-agent: AdsBot-Google
This bot is responsible for Google Ads. The same rules as for the general and Googlebot apply.

User-agent: Screaming Frog SEO Spider
All pages are allowed for this bot, which is commonly used for SEO audits.

User-agent: EtaoSpider
All access is disallowed for this bot.

User-agent: GPTBot
Access is disallowed for GPTBot, a crawler used for AI models.

User-agent: CCBot
All access is disallowed for this bot as well.

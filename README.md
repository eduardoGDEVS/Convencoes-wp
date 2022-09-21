### Padrões de desenvolvimento com WordPress.

### Database

Començando pela convenção mais simples, os padrões para nomenclaturas de bancos de dados ficam assim:

**Título do banco**: {*nome-do-projeto ou cliente*}-{*tipo-do-projeto*}-wordpress <br>
`Tipo do projeto: cms, api, site, etc` `Ex: netflix-api-wordpress, disney-promocao-natal-wordpress`

**Prefixo das tabelas**: wp_{*nome-do-projeto ou cliente*}_

---

### Front-end

**Artigo: CSS Coding Standards**<br>
[Acesso ao link](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/css/)

**Artigo: HTML Coding Standards**<br>
[Acesso ao link](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/html/)

**Artigo: JavaScript Coding Standards**<br>
[Acesso ao link](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/javascript/)

---

### Back-end

**Artigo: PHP Coding Standards**<br>
[Acesso ao link](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/php/)

---

### Estrutura das pastas do tema

**wp-content/themes/{*nome-do-projeto*}/**
- assets/
  - css/
  - images/ `Apenas imagens estáticas`
  - js/
  - vendor/ `Plugins e bibliotecas importados`
- inc/
  - customizer/
    - register.php
    - scripts-and-styles.php `JS e CSS do customizer`
    - constants.php `Para gravar em constantes os valoes obtidos do customizer`
  - actions.php
  - filters.php
  - scripts-and-styles.php `JS e CSS do tema`
  - config.php `Acidiona os suportes a menus, thumbnails e posts, além de outras configurações básicas necessárias.`
  - api.php `Opcional. Apenas para incluir os arquivos de configuração das api's da pasta **wp-content/api**`
- template-parts/
  - global/ 
  - footer/
  - header/
  - navigation/
  - modals/
  - forms/
  - page/
  - post/
  - *podemos também ter pastas para cada **post_type** cadastrado.*
- templates/ `Templates para posts ou páginas`
  
**wp-content/admin**
- config/
  - post-types.php
  - settings-pages.php `Opcional, no caso de opções avançadas em que o customizer.php não seja suportado.`
  - scripts-and-styles.php `Para adicionar js e css no admin.`
  - menu-pages-and-items.php `Para adicionar itens no menu e novas páginas ao admin.`
  - templates/ `Contendo arquivos que alteram a estrutura do admin como a dashboard (ex: dashboard.php)`
  - assets/
    - css/
    - images/
    - js/
    - vendor/ 
- wp-api/ `Opcional. Usado para configuração ou alteração da RESTApi padrão do WP`
- api/ `Opcional. Contém arquivos para configuração e uso de apis externas` 
    
**Artigo: Organizing front end files and folders**<br>
[Acesso ao link](https://developer.wordpress.org/themes/basics/organizing-theme-files/)

---

### Próximos passos:
https://developer.wordpress.org/plugins/security/securing-output/<br>
https://phpqa.io/projects/phpcbf.html<br>
https://www.digitalocean.com/community/tutorials/how-to-install-wordpress-with-docker-compose-pt


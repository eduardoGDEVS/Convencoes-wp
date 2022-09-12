### GD Padrões de desenvolvimento.

## Front-end

### Artigo: CSS Coding Standards
[Acesso ao link](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/css/)

### Artigo: HTML Coding Standards
[Acesso ao link](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/css/)

### Artigo: JavaScript Coding Standards
[Acesso ao link](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/javascript/)

---

## Back-end

### Artigo: PHP Coding Standards
[Acesso ao link](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/php/)

---

### Estrutura das pastas do tema

**wp-content/themes/*nome-do-projeto*/**
- assets/
  - css/
  - images/ `Apenas imagens estáticas`
  - js/
  - vendor/ `Plugins e bibliotecas importados`
- inc/
  - customizer/
    - register.php
    - scripts-and-styles.php
    - constants.php `Para gravar em constantes os valoes obtidos do customizer`
  - actions.php
  - filters.php
  - api.php `Opcional. Apenas para incluir os arquivos de configuração das api's da pasta **wp-content/api**`
- template-parts/
  - footer/
  - header/
  - navigation/
  - page/
  - post/
  - *podemos também ter pastas para cada **post_type** cadastrado.*
- templates/ `Templates para posts ou páginas`
  
**wp-content/**
- admin/
  - settings-pages.php `Opcional, no caso de opções avançadas em que o customizer.php não seja suportado.`
  - post-types.php
  - menu-items.php
  - scripts-and-styles.php
  - customizer.php 
- wp-api/ `Opcional. Usado para configuração ou alteração da RESTApi padrão do WP`
- api/ `Opcional. Contém arquivos para configuração e uso de apis externas` 
    
**Artigo: Organizing front end files and folders**<br>
[Acesso ao link](https://developer.wordpress.org/themes/basics/organizing-theme-files/)

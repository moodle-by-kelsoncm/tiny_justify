# Guia de Uso & Desenvolvimento — moodle-tiny_justify

## Guia de Uso

1. Abra qualquer área de texto que utilize o editor TinyMCE no Moodle.
2. Selecione o texto ou parágrafo que deseja justificar.
3. Clique no botão **Justify** na barra de ferramentas.

---

## Desenvolvimento & Build AMD

Se você modificar arquivos dentro de `amd/src/` (`plugin.js`, `commands.js`, `configuration.js`):

1. Atualize a versão em `version.php`.
2. Compile os módulos AMD com Grunt na raiz do Moodle:
   ```bash
   npx grunt amd --root=lib/editor/tiny/plugins/justify
   ```
3. Limpe os caches via CLI ou painel de administração:
   ```bash
   php admin/cli/purge_caches.php
   ```

## `web` Generator

The `web` generator transforms JSX AST entries into complete web bundles, producing server-side rendered HTML pages, client-side JavaScript with code splitting, and bundled CSS styles.

### Configuring

The `web` generator accepts the following configuration options:

| Name           | Type     | Default                                             | Description                                                           |
| -------------- | -------- | --------------------------------------------------- | --------------------------------------------------------------------- |
| `output`       | `string` | -                                                   | The directory where HTML, JavaScript, and CSS files will be written   |
| `templatePath` | `string` | `'template.html'`                                   | Path to the HTML template file                                        |
| `imports`      | `object` | [See Default Theme Imports](#default-theme-imports) | Object mapping import aliases to component paths for custom branding. |

#### Default Theme Imports

By default, the `web` generator uses the Node.js branding. These aliases can be overridden in your `doc-kit.config.mjs`:

| Alias               | Default Path                                 |
| ------------------- | -------------------------------------------- |
| `#theme/Logo`       | `@node-core/ui-components/Common/NodejsLogo` |
| `#theme/Navigation` | `src/generators/web/ui/components/NavBar`    |
| `#theme/Sidebar`    | `src/generators/web/ui/components/SideBar`   |
| `#theme/MetaBar`    | `src/generators/web/ui/components/MetaBar`   |

# WPGatsby

WPGatsby is a free open-source WordPress plugin that optimizes your WordPress site to work as a data source for [Gatsby](https://www.gatsbyjs.com/docs/how-to/sourcing-data/sourcing-from-wordpress).

This plugin must be used in combination with the npm package [`gatsby-source-wordpress@^4.0.0`](https://www.npmjs.com/package/gatsby-source-wordpress).

## Install and Activation

WPGatsby is available on the WordPress.org repository and can be installed from your WordPress dashboard, or by using any other plugin installation method you prefer, such as installing with Composer from wpackagist.org.

## Enhanced Build Control Features

This fork adds two important features to help manage Gatsby build API limits:

1. **Enable/Disable Build Webhook** - Temporarily disable builds during bulk content updates to avoid triggering unnecessary builds.

2. **Trigger Build Now** - Manually trigger a build on demand after completing bulk updates or when re-enabling the build webhook.

These features are especially useful for sites with build limitations or when performing multiple content changes.

## Plugin Overview

This plugin has 2 primary responsibilities:

- [Monitor Activity in WordPress to keep Gatsby in sync with WP](https://github.com/gatsbyjs/wp-gatsby/blob/master/docs/action-monitor.md)
- [Configure WordPress Previews to work with Gatsby](https://github.com/gatsbyjs/gatsby/blob/master/packages/gatsby-source-wordpress/docs/tutorials/configuring-wp-gatsby.md#setting-up-preview)

Additionally, WPGatsby has a settings page to connect your WordPress site with your Gatsby site:

- [WPGatsby Settings](https://github.com/gatsbyjs/gatsby/blob/master/packages/gatsby-source-wordpress/docs/tutorials/configuring-wp-gatsby.md)

## Changelog

### 2.3.4

- Added "Enable Build Webhook" toggle to allow temporarily disabling builds during bulk content updates
- Added "Trigger Build Now" option to manually trigger builds on demand
- Improved build control for better management of Gatsby build API limits

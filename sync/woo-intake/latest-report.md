# Future Woo intake report

Generated: 2026-10-27
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-10-20`.
- Design-facing labels, paths, keywords, tracked people, and explicitly tracked PRs.
- Future Woo feature flags that should be forced on for the prototype.

## Gate checks

- pass: Intake tests
- pass: Build
- pass: PHP syntax

## Feature flags Future Woo will force-enable

- Products table: DataViews: product_list_dataviews, products_table_dataviews
  Designer review path: Products > All Products
- Nested admin navigation: navigation_v2
  Designer review path: WooCommerce admin rail

## Woo candidates

### #64712 Add nested admin navigation behind navigation_v2 feature flag
https://github.com/woocommerce/woocommerce/pull/64712

Score: 12
Author: beaulebens
Source search: All recent Woo PR activity: updated:>=2026-10-20; Tracked PR: Nested admin navigation
Why it matched: path: plugins/woocommerce/src/Internal/Admin/Navigation; path: plugins/woocommerce/client/legacy/js/admin/admin-navigation-v2.js; path: plugins/woocommerce/client/legacy/css/admin-navigation-v2.scss; keyword: feature flag; keyword: experiment; keyword: navigation; tracked PR: Nested admin navigation
Touched areas:
- .gitignore
- docs/best-practices/nested-admin-navigation.md
- packages/js/experimental-products-app/src/product-edit/utils.ts
- plugins/woocommerce/changelog/dev-native-rail-rendering
- plugins/woocommerce/changelog/feat-nested-admin-navigation
- plugins/woocommerce/client/legacy/css/admin-navigation-v2.scss
- plugins/woocommerce/client/legacy/js/admin/admin-navigation-v2.js
- plugins/woocommerce/includes/class-woocommerce.php

### #70106 Retire the experimental Settings UI
https://github.com/woocommerce/woocommerce/pull/70106

Score: 11
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-10-20
Why it matched: path: plugins/woocommerce/client/admin/client/settings; path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment
Touched areas:
- .github/project-community-pr-assigner.json
- .syncpackrc
- docs/extensions/settings-and-config/extend-wc-settings-page.md
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/dependency-extraction-webpack-plugin/assets/packages.js
- packages/js/dependency-extraction-webpack-plugin/changelog/remove-settings-ui
- packages/js/payment-settings/build

### #69173 Remove the experimental Settings UI JS
https://github.com/woocommerce/woocommerce/pull/69173

Score: 11
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-10-20
Why it matched: path: plugins/woocommerce/client/admin/client/settings; keyword: dataviews; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment
Touched areas:
- .github/project-community-pr-assigner.json
- .syncpackrc
- packages/js/dependency-extraction-webpack-plugin/assets/packages.js
- packages/js/dependency-extraction-webpack-plugin/changelog/remove-settings-ui
- packages/js/settings-ui/README.md
- packages/js/settings-ui/build.mjs
- packages/js/settings-ui/changelog/add-settings-ui
- packages/js/settings-ui/changelog/add-shell-header-fields

### #69172 Deprecate the experimental Settings UI PHP classes
https://github.com/woocommerce/woocommerce/pull/69172

Score: 8
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-10-20
Why it matched: path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: experiment
Touched areas:
- plugins/woocommerce/changelog/remove-settings-ui-php
- plugins/woocommerce/includes/admin/class-wc-admin-settings.php
- plugins/woocommerce/includes/admin/settings/class-wc-settings-page.php
- plugins/woocommerce/includes/admin/settings/class-wc-settings-products.php
- plugins/woocommerce/includes/admin/views/html-admin-settings.php
- plugins/woocommerce/src/Admin/Settings/AGENTS.md
- plugins/woocommerce/src/Admin/Settings/LegacySettingsPageAdapter.php
- plugins/woocommerce/src/Admin/Settings/SettingsSection.php

### #67808 Add stock notification emails as WC_Email classes
https://github.com/woocommerce/woocommerce/pull/67808

Score: 7
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-10-20
Why it matched: path: plugins/woocommerce/includes/admin; keyword: stock notification; keyword: email template; author: j111q
Touched areas:
- plugins/woocommerce/changelog/29389-stock-notification-emails
- plugins/woocommerce/includes/admin/settings/class-wc-settings-products.php
- plugins/woocommerce/includes/class-wc-emails.php
- plugins/woocommerce/includes/emails/class-wc-email-backorder.php
- plugins/woocommerce/includes/emails/class-wc-email-low-stock.php
- plugins/woocommerce/includes/emails/class-wc-email-no-stock.php
- plugins/woocommerce/templates/emails/backorder.php
- plugins/woocommerce/templates/emails/low-stock.php

### #69174 Remove the Settings UI docs
https://github.com/woocommerce/woocommerce/pull/69174

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-10-20
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: experiment
Touched areas:
- docs/extensions/settings-and-config/extend-wc-settings-page.md
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md

### #68545 WIP: Settings UI - Switch to opt-out by default
https://github.com/woocommerce/woocommerce/pull/68545

Score: 6
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-10-20
Why it matched: path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui
Touched areas:
- docs/extensions/settings-and-config/extend-wc-settings-page.md
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/README.md
- packages/js/settings-ui/src/dataform-adapter.tsx
- packages/js/settings-ui/src/hidden-inputs.tsx
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/dataform-adapter.test.tsx

### #65788 Migrate customer stock notification screens to the order actions "more actions" menu
https://github.com/woocommerce/woocommerce/pull/65788

Score: 5
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-10-20
Why it matched: path: plugins/woocommerce/includes/admin; keyword: stock notification; author: j111q
Touched areas:
- plugins/woocommerce/changelog/64564-sprinkle-order-edit-wp7-alignment
- plugins/woocommerce/changelog/update-stock-notification-actions-more-menu
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/client/legacy/js/admin/order-actions-menu.js
- plugins/woocommerce/client/legacy/js/admin/wc-customer-stock-notifications.js
- plugins/woocommerce/includes/admin/class-wc-admin-assets.php
- plugins/woocommerce/includes/admin/meta-boxes/class-wc-meta-box-order-actions.php

### #68801 Document the three site visibility states for integrators
https://github.com/woocommerce/woocommerce/pull/68801

Score: 4
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-10-20
Why it matched: keyword: feature flag; author: j111q
Touched areas:
- docs/extensions/extension-onboarding/integrating-coming-soon-mode.md

### #66142 Add TreeSelect prototype source references
https://github.com/woocommerce/woocommerce/pull/66142

Score: 4
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-10-20
Why it matched: keyword: rsm; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/add-treeselect-prototype-source-reference
- plugins/woocommerce/docs/superpowers/prototypes/tree-select/README.md
- plugins/woocommerce/docs/superpowers/prototypes/tree-select/source/components/ProductCategoryTreeCombo.jsx.txt
- plugins/woocommerce/docs/superpowers/prototypes/tree-select/source/components/TreeCombo.jsx.txt
- plugins/woocommerce/docs/superpowers/prototypes/tree-select/source/components/TreeComboLab.jsx.txt
- plugins/woocommerce/docs/superpowers/prototypes/tree-select/source/data/countryTree.js.txt
- plugins/woocommerce/docs/superpowers/prototypes/tree-select/source/data/productCategoryTree.js.txt
- plugins/woocommerce/docs/superpowers/prototypes/tree-select/source/styles.treecombo-excerpt.css

### #70013 [Backport to release/11.3] Show marketing channels to site admins on multisite
https://github.com/woocommerce/woocommerce/pull/70013

Score: 3
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-10-20
Why it matched: path: plugins/woocommerce/client/admin/client/marketing; keyword: marketing channels
Touched areas:
- plugins/woocommerce/changelog/55130-marketing-channels-multisite-site-admin
- plugins/woocommerce/client/admin/client/marketing/hooks/useRecommendedChannels.ts
- plugins/woocommerce/src/Internal/Admin/Marketing.php

### #69993 Show marketing channels to site admins on multisite
https://github.com/woocommerce/woocommerce/pull/69993

Score: 3
Author: yuliyan
Source search: All recent Woo PR activity: updated:>=2026-10-20
Why it matched: path: plugins/woocommerce/client/admin/client/marketing; keyword: marketing channels
Touched areas:
- plugins/woocommerce/changelog/55130-marketing-channels-multisite-site-admin
- plugins/woocommerce/client/admin/client/marketing/hooks/useRecommendedChannels.ts
- plugins/woocommerce/src/Internal/Admin/Marketing.php

## Surface ownership policy

### Marketing and sales channels
Mode: vision-owned
Owner: Future Woo design
Woo PR: #70013 [Backport to release/11.3] Show marketing channels to site admins on multisite
Intent: default
Action: report-only
Designer review path: Marketing > Campaigns
Matched by: path: plugins/woocommerce/client/admin/client/marketing; keyword: marketing channels
Auto-apply: skipped; this stays visible without overwriting the Future Woo surface.
- Protects the future-facing Marketing > Campaigns exploration while still surfacing useful Woo changes.

### Marketing and sales channels
Mode: vision-owned
Owner: Future Woo design
Woo PR: #69993 Show marketing channels to site admins on multisite
Intent: bugfix
Action: report-only
Designer review path: Marketing > Campaigns
Matched by: path: plugins/woocommerce/client/admin/client/marketing; keyword: marketing channels
Auto-apply: skipped; this stays visible without overwriting the Future Woo surface.
- Protects the future-facing Marketing > Campaigns exploration while still surfacing useful Woo changes.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #70106 Retire the experimental Settings UI
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/client/admin/client/settings; path: plugins/woocommerce/includes/admin/settings; keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #69173 Remove the experimental Settings UI JS
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/client/admin/client/settings; keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #69172 Deprecate the experimental Settings UI PHP classes
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings; keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #67808 Add stock notification emails as WC_Email classes
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #69174 Remove the Settings UI docs
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #68545 WIP: Settings UI - Switch to opt-out by default
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings; keyword: settings-ui; keyword: settings ui
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Woo admin navigation
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #64712 Add nested admin navigation behind navigation_v2 feature flag
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce admin rail
Matched by: path: plugins/woocommerce/src/Internal/Admin/Navigation; path: plugins/woocommerce/client/legacy/js/admin/admin-navigation-v2.js; path: plugins/woocommerce/client/legacy/css/admin-navigation-v2.scss; keyword: navigation_v2; keyword: nested admin navigation; keyword: navigation
Auto-merge: held; the bot should leave a draft PR for review.
- Navigation changes touch the frame of the whole prototype, so feature-flagged UI shifts should pause for review.

## Patch adapters

No patch adapters matched this run.

## Designer review paths

- Products > All Products
- WooCommerce admin rail
- Marketing > Campaigns
- WooCommerce > Settings

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

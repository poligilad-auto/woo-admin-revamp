# Future Woo intake report

Generated: 2026-07-07
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-06-30`.
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
Source search: Tracked PR: Nested admin navigation
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

### #65975 Add native Settings UI page provider for registered sections
https://github.com/woocommerce/woocommerce/pull/65975

Score: 10
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-06-30
Why it matched: path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: navigation
Touched areas:
- docs/extensions/settings-and-config/settings-ui.md
- plugins/woocommerce/changelog/add-settings-section-ui-page-provider
- plugins/woocommerce/changelog/add-settings-ui-default-section-navigation
- plugins/woocommerce/changelog/fix-66031-settings-ui-registry-resolution-guard
- plugins/woocommerce/includes/admin/views/html-admin-settings.php
- plugins/woocommerce/src/Admin/Settings/SettingsSection.php
- plugins/woocommerce/src/Admin/Settings/SettingsSectionUIPageProviderInterface.php
- plugins/woocommerce/src/Admin/Settings/SettingsUIPageInterface.php

### #64476 Order notes meta box: clarify visibility, modernize bubble styling
https://github.com/woocommerce/woocommerce/pull/64476

Score: 7
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-06-30
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit; keyword: email template; author: j111q
Touched areas:
- plugins/woocommerce/changelog/64999-sprinkle-order-notes-visibility
- plugins/woocommerce/client/legacy/css/_variables.scss
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/includes/admin/class-wc-admin-assets.php
- plugins/woocommerce/includes/admin/meta-boxes/class-wc-meta-box-order-notes.php
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-notes.php
- plugins/woocommerce/includes/class-wc-ajax.php

### #66232 Keep Settings UI field values in the schema's value vocabulary
https://github.com/woocommerce/woocommerce/pull/66232

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-06-30
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag
Touched areas:
- packages/js/settings-ui/changelog/fix-checkbox-value-vocabulary
- packages/js/settings-ui/changelog/fix-preserve-initial-value-representation
- packages/js/settings-ui/src/hidden-inputs.tsx
- packages/js/settings-ui/src/native-fields.tsx
- packages/js/settings-ui/src/registry.ts
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/html-rendering.test.tsx
- packages/js/settings-ui/src/test/native-fields.test.tsx

### #65788 Migrate customer stock notification screens to the order actions "more actions" menu
https://github.com/woocommerce/woocommerce/pull/65788

Score: 5
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-06-30
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

### #65636 Add deprecated WC Admin feature flag shims
https://github.com/woocommerce/woocommerce/pull/65636

Score: 5
Author: gigitux
Source search: All recent Woo PR activity: updated:>=2026-06-30
Why it matched: path: plugins/woocommerce/src/Admin; keyword: settings-ui; keyword: feature flag
Touched areas:
- plugins/woocommerce/changelog/dev-deflag-wc-admin-feature-compatibility-shims
- plugins/woocommerce/client/admin/client/typings/global.d.ts
- plugins/woocommerce/client/admin/client/utils/features/features.ts
- plugins/woocommerce/client/admin/client/utils/features/retired-feature-flags.ts
- plugins/woocommerce/client/admin/client/utils/test/admin-settings.js
- plugins/woocommerce/client/admin/package.json
- plugins/woocommerce/src/Admin/Features/Features.php
- plugins/woocommerce/src/Blocks/BlockPatterns.php

### #64564 Align Order Edit meta boxes with WordPress 7.0 design conventions
https://github.com/woocommerce/woocommerce/pull/64564

Score: 5
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-06-30
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit; author: j111q
Touched areas:
- plugins/woocommerce/changelog/64564-sprinkle-order-edit-wp7-alignment
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/includes/admin/meta-boxes/class-wc-meta-box-order-actions.php
- plugins/woocommerce/includes/admin/meta-boxes/class-wc-meta-box-order-data.php

### #66142 Add TreeSelect prototype source references
https://github.com/woocommerce/woocommerce/pull/66142

Score: 4
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-06-30
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

### #66110 Fix duplicate shipping marketplace link
https://github.com/woocommerce/woocommerce/pull/66110

Score: 4
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-06-30
Why it matched: path: plugins/woocommerce/client/admin/client/shipping; path: plugins/woocommerce/includes/admin; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/fix-duplicate-shipping-marketplace-link
- plugins/woocommerce/client/admin/client/shipping/experimental-shipping-recommendations.tsx
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations.scss
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations.tsx
- plugins/woocommerce/client/admin/client/shipping/test/experimental-shipping-recommendations.tsx
- plugins/woocommerce/includes/admin/views/html-admin-settings.php
- plugins/woocommerce/tests/php/includes/admin/views/class-wc-admin-settings-view-test.php

### #66042 Update Settings UI container radius
https://github.com/woocommerce/woocommerce/pull/66042

Score: 4
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-06-30
Why it matched: keyword: settings-ui; keyword: settings ui
Touched areas:
- plugins/woocommerce/changelog/wooprd-3555-settings-container-radius
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/settings-ui.scss

### #65657 Add POS staff foundation: feature flag, orchestrator, caps model
https://github.com/woocommerce/woocommerce/pull/65657

Score: 4
Author: jaclync
Source search: All recent Woo PR activity: updated:>=2026-06-30
Why it matched: keyword: feature flag; keyword: experiment
Touched areas:
- plugins/woocommerce/changelog/add-pos-staff-foundation
- plugins/woocommerce/includes/class-woocommerce.php
- plugins/woocommerce/src/Internal/Features/FeaturesController.php
- plugins/woocommerce/src/Internal/POS/Capabilities.php
- plugins/woocommerce/src/Internal/POS/POSController.php
- plugins/woocommerce/tests/php/src/Internal/POS/CapabilitiesTest.php

### #64439 Add My Account tab for Back in Stock Notifications (RSM-444)
https://github.com/woocommerce/woocommerce/pull/64439

Score: 4
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-06-30
Why it matched: keyword: rsm; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/bis-features-screen-toggle
- plugins/woocommerce/includes/class-woocommerce.php
- plugins/woocommerce/src/Internal/DataStores/StockNotifications/StockNotificationsDataStore.php
- plugins/woocommerce/src/Internal/Features/FeaturesController.php
- plugins/woocommerce/src/Internal/StockNotifications/Frontend/MyAccountEndpoint.php
- plugins/woocommerce/src/Internal/StockNotifications/NotificationQuery.php
- plugins/woocommerce/src/Internal/StockNotifications/StockNotifications.php
- plugins/woocommerce/templates/myaccount/stock-notifications.php

### #66348 Add warnings for shadowed shipping zones
https://github.com/woocommerce/woocommerce/pull/66348

Score: 3
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-06-30
Why it matched: path: plugins/woocommerce/includes/admin; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/30340-shipping-zone-order-warning
- plugins/woocommerce/includes/admin/settings/class-wc-settings-shipping.php
- plugins/woocommerce/includes/admin/settings/views/html-admin-page-shipping-zones.php
- plugins/woocommerce/includes/class-wc-ajax.php
- plugins/woocommerce/includes/class-wc-shipping-zones.php
- plugins/woocommerce/tests/php/includes/class-wc-shipping-zones-test.php

### #66119 Hide Downloadable product permissions metabox by default on the order edit screen
https://github.com/woocommerce/woocommerce/pull/66119

Score: 3
Author: mikejolley
Source search: All recent Woo PR activity: updated:>=2026-06-30
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit
Touched areas:
- plugins/woocommerce/changelog/dsgwoo-1343-hide-downloads-metabox
- plugins/woocommerce/includes/admin/class-wc-admin-post-types.php
- plugins/woocommerce/phpstan-baseline.neon
- plugins/woocommerce/tests/e2e/tests/order/order-edit.spec.ts
- plugins/woocommerce/tests/unit-tests/admin/class-wc-tests-admin-post-types.php

## Surface ownership policy

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #65975 Add native Settings UI page provider for registered sections
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66232 Keep Settings UI field values in the schema's value vocabulary
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66042 Update Settings UI container radius
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66348 Add warnings for shadowed shipping zones
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Shipping providers
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #66110 Fix duplicate shipping marketplace link
Intent: bugfix
Action: self-merge
Designer review path: WooCommerce > Settings > Shipping
Matched by: path: plugins/woocommerce/client/admin/client/shipping
- Shipping provider work can follow the same provider-card pattern, but design-facing reshapes should stop as drafts.

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
- WooCommerce > Settings
- WooCommerce > Settings > Shipping

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

# Future Woo intake report

Generated: 2026-08-25
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-08-18`.
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

### #67864 Remove obsolete Settings UI styles
https://github.com/woocommerce/woocommerce/pull/67864

Score: 8
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: keyword: dataviews; keyword: settings-ui; keyword: settings ui; keyword: experiment
Touched areas:
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/README.md
- packages/js/settings-ui/changelog/add-wooprd-3595-dataform-adapter
- packages/js/settings-ui/changelog/fix-number-custom-attributes
- packages/js/settings-ui/changelog/fix-number-spin-control-scientific-precision
- packages/js/settings-ui/changelog/update-number-spin-control
- packages/js/settings-ui/changelog/update-remove-woo-field-renderers

### #67334 Validate Settings UI schemas before rendering
https://github.com/woocommerce/woocommerce/pull/67334

Score: 8
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: feature flag
Touched areas:
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/changelog/fix-wooprd-3593-missing-components
- packages/js/settings-ui/src/native-fields.tsx
- packages/js/settings-ui/src/registry.ts
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/html-rendering.test.tsx
- packages/js/settings-ui/src/test/native-fields.test.tsx

### #64490 Move Back in Stock Notifications activation from wp-config flag to a Features setting
https://github.com/woocommerce/woocommerce/pull/64490

Score: 8
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: keyword: settings ui; keyword: feature flag; keyword: experiment; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/bis-features-screen-toggle
- plugins/woocommerce/includes/class-wc-install.php
- plugins/woocommerce/includes/class-woocommerce.php
- plugins/woocommerce/includes/wc-update-functions.php
- plugins/woocommerce/phpstan-baseline.neon
- plugins/woocommerce/src/Internal/DataStores/StockNotifications/StockNotificationsDataStore.php
- plugins/woocommerce/src/Internal/Features/FeaturesController.php
- plugins/woocommerce/src/Internal/StockNotifications/StockNotifications.php

### #67808 Add stock notification emails as WC_Email classes
https://github.com/woocommerce/woocommerce/pull/67808

Score: 7
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-08-18
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

### #67726 Remove experimental abandoned cart recovery feature
https://github.com/woocommerce/woocommerce/pull/67726

Score: 7
Author: senadir
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: path: plugins/woocommerce/src/Admin; keyword: feature flag; keyword: experiment; keyword: rsm
Touched areas:
- .github/project-community-pr-assigner.yml
- plugins/woocommerce/changelog/remove-abandoned-cart-recovery-feature
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/abandoned-cart-recovery-recommendations-wrapper.tsx
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/abandoned-cart-recovery-recommendations.scss
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/abandoned-cart-recovery-recommendations.tsx
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/automatewoo-item.tsx
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/index.ts
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/mailpoet-item.tsx

### #67909 [Backport to release/11.1] Remove experimental products app features
https://github.com/woocommerce/woocommerce/pull/67909

Score: 6
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: keyword: dataviews; keyword: feature flag; keyword: experiment
Touched areas:
- .github/project-community-pr-assigner.yml
- .syncpackrc
- packages/js/dependency-extraction-webpack-plugin/assets/packages.js
- packages/js/dependency-extraction-webpack-plugin/changelog/remove-experimental-products-app
- packages/js/experimental-products-app/.npmrc
- packages/js/experimental-products-app/README.md
- packages/js/experimental-products-app/babel.config.js
- packages/js/experimental-products-app/blueprint.json

### #67883 Remove experimental products app features
https://github.com/woocommerce/woocommerce/pull/67883

Score: 6
Author: gigitux
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: keyword: dataviews; keyword: feature flag; keyword: experiment
Touched areas:
- .github/project-community-pr-assigner.yml
- .syncpackrc
- packages/js/dependency-extraction-webpack-plugin/assets/packages.js
- packages/js/dependency-extraction-webpack-plugin/changelog/remove-experimental-products-app
- packages/js/experimental-products-app/.npmrc
- packages/js/experimental-products-app/README.md
- packages/js/experimental-products-app/babel.config.js
- packages/js/experimental-products-app/blueprint.json

### #67865 Remove card header actions from the Settings UI schema
https://github.com/woocommerce/woocommerce/pull/67865

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: experiment
Touched areas:
- packages/js/settings-ui/changelog/update-remove-group-actions
- packages/js/settings-ui/src/index.ts
- packages/js/settings-ui/src/types.ts
- plugins/woocommerce/changelog/dev-remove-settings-ui-group-actions
- plugins/woocommerce/src/Internal/Admin/Settings/SettingsUISchema.php
- plugins/woocommerce/tests/php/src/Internal/Admin/Settings/SettingsUISchemaTest.php

### #67863 Remove Woo-owned Settings UI field renderers
https://github.com/woocommerce/woocommerce/pull/67863

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: experiment
Touched areas:
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/README.md
- packages/js/settings-ui/changelog/fix-number-custom-attributes
- packages/js/settings-ui/changelog/fix-number-spin-control-scientific-precision
- packages/js/settings-ui/changelog/update-number-spin-control
- packages/js/settings-ui/changelog/update-remove-woo-field-renderers
- packages/js/settings-ui/package.json
- packages/js/settings-ui/src/dataform-adapter.tsx

### #67846 Add a DataForm adapter for the Settings UI schema
https://github.com/woocommerce/woocommerce/pull/67846

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: keyword: dataviews; keyword: settings-ui; keyword: settings ui
Touched areas:
- packages/js/settings-ui/changelog/add-wooprd-3595-dataform-adapter
- packages/js/settings-ui/src/dataform-adapter.tsx
- packages/js/settings-ui/src/test/dataform-adapter.test.tsx

### #66039 Add search and pagination to order tax modal
https://github.com/woocommerce/woocommerce/pull/66039

Score: 5
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit; author: j111q
Touched areas:
- plugins/woocommerce/changelog/add-tax-rate-modal-search-pagination
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/includes/admin/class-wc-admin-assets.php
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-items.php
- plugins/woocommerce/includes/class-wc-ajax.php
- plugins/woocommerce/tests/php/includes/class-wc-ajax-test.php

### #67335 Canonicalize Settings UI values before rendering
https://github.com/woocommerce/woocommerce/pull/67335

Score: 4
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: keyword: settings-ui; keyword: settings ui
Touched areas:
- packages/js/settings-ui/changelog/fix-wooprd-3594-settings-value-boundary
- packages/js/settings-ui/package.json
- packages/js/settings-ui/src/hidden-inputs.tsx
- packages/js/settings-ui/src/native-fields.tsx
- packages/js/settings-ui/src/number-spin-control.tsx
- packages/js/settings-ui/src/registry.ts
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/hidden-inputs.test.ts

### #64482 Add Playwright e2e coverage for BIS alpha
https://github.com/woocommerce/woocommerce/pull/64482

Score: 4
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: keyword: rsm; keyword: stock notification
Touched areas:
- .markdownlintignore
- plugins/woocommerce/.wp-env.e2e.json
- plugins/woocommerce/changelog/rsm-437-bis-playwright-coverage
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/tests/e2e/bin/test-env-setup.sh
- plugins/woocommerce/tests/e2e/playwright.config.ts
- plugins/woocommerce/tests/e2e/test-plugins/woocommerce-bis-test-helper/woocommerce-bis-test-helper.php
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/README.md

### #64289 Add experimental Edge Cache Support for cart, checkout and mini-cart blocks
https://github.com/woocommerce/woocommerce/pull/64289

Score: 4
Author: jbouganim
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: keyword: feature flag; keyword: experiment
Touched areas:
- docs/apis/store-api/resources-endpoints/checkout.md
- docs/best-practices/performance/configuring-caching-plugins.md
- plugins/woocommerce/changelog/64289-feature-edge-caching-phase-1
- plugins/woocommerce/client/blocks/assets/js/base/components/skeleton/patterns/checkout/index.tsx
- plugins/woocommerce/client/blocks/assets/js/base/stores/woocommerce/cart.ts
- plugins/woocommerce/client/blocks/assets/js/blocks/checkout/block.tsx
- plugins/woocommerce/client/blocks/assets/js/data/cart/resolvers.ts
- plugins/woocommerce/client/blocks/assets/js/data/checkout/action-types.ts

### #67921 Fix negative quantity validation in the admin order editor
https://github.com/woocommerce/woocommerce/pull/67921

Score: 3
Author: ralucastan
Source search: All recent Woo PR activity: updated:>=2026-08-18
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit
Touched areas:
- plugins/woocommerce/changelog/fix-31068-order-item-qty-validation
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-item.php
- plugins/woocommerce/includes/class-wc-ajax.php
- plugins/woocommerce/src/Internal/Admin/Orders/ItemQuantityLimits.php
- plugins/woocommerce/tests/e2e/tests/order/order-item-quantity-validation.spec.ts
- plugins/woocommerce/tests/php/includes/class-wc-ajax-test.php
- plugins/woocommerce/tests/php/src/Internal/Admin/Orders/ItemQuantityLimitsTest.php

## Surface ownership policy

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #67864 Remove obsolete Settings UI styles
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #67334 Validate Settings UI schemas before rendering
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings; keyword: settings ui
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
Woo PR: #67865 Remove card header actions from the Settings UI schema
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #67863 Remove Woo-owned Settings UI field renderers
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #67846 Add a DataForm adapter for the Settings UI schema
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #67335 Canonicalize Settings UI values before rendering
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
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
- WooCommerce > Settings

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

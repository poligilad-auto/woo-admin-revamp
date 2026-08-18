# Future Woo intake report

Generated: 2026-08-18
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-08-11`.
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

### #67369 Load DataViews 17.1.0 safely for the new Settings UI
https://github.com/woocommerce/woocommerce/pull/67369

Score: 8
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-08-11
Why it matched: keyword: dataviews; keyword: settings-ui; keyword: settings ui; keyword: experiment
Touched areas:
- .syncpackrc
- packages/js/settings-ui/changelog/fix-dataviews-17-wordpress-69-compatibility
- packages/js/settings-ui/package.json
- packages/js/settings-ui/src/dataform-runtime.ts
- packages/js/settings-ui/src/dataviews-wp.d.ts
- packages/js/settings-ui/src/native-fields.tsx
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/style.scss

### #67334 Validate Settings UI schemas before rendering
https://github.com/woocommerce/woocommerce/pull/67334

Score: 8
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-08-11
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
Source search: All recent Woo PR activity: updated:>=2026-08-11
Why it matched: keyword: settings ui; keyword: feature flag; keyword: experiment; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/bis-features-screen-toggle
- plugins/woocommerce/includes/class-woocommerce.php
- plugins/woocommerce/src/Internal/DataStores/StockNotifications/StockNotificationsDataStore.php
- plugins/woocommerce/src/Internal/Features/FeaturesController.php
- plugins/woocommerce/tests/legacy/bootstrap.php

### #67726 Remove experimental abandoned cart recovery feature
https://github.com/woocommerce/woocommerce/pull/67726

Score: 7
Author: senadir
Source search: All recent Woo PR activity: updated:>=2026-08-11
Why it matched: path: plugins/woocommerce/src/Admin; keyword: feature flag; keyword: experiment; keyword: rsm
Touched areas:
- plugins/woocommerce/changelog/remove-abandoned-cart-recovery-feature
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/abandoned-cart-recovery-recommendations-wrapper.tsx
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/abandoned-cart-recovery-recommendations.scss
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/abandoned-cart-recovery-recommendations.tsx
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/automatewoo-item.tsx
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/index.ts
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/mailpoet-item.tsx
- plugins/woocommerce/client/admin/client/abandoned-cart-recovery/test/abandoned-cart-recovery-recommendations-wrapper.test.tsx

### #67335 Canonicalize Settings UI values before rendering
https://github.com/woocommerce/woocommerce/pull/67335

Score: 5
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-08-11
Why it matched: path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui
Touched areas:
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/changelog/fix-wooprd-3593-missing-components
- packages/js/settings-ui/changelog/fix-wooprd-3594-settings-value-boundary
- packages/js/settings-ui/package.json
- packages/js/settings-ui/src/hidden-inputs.tsx
- packages/js/settings-ui/src/native-fields.tsx
- packages/js/settings-ui/src/registry.ts

### #66039 Add search and pagination to order tax modal
https://github.com/woocommerce/woocommerce/pull/66039

Score: 5
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-08-11
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit; author: j111q
Touched areas:
- plugins/woocommerce/changelog/add-tax-rate-modal-search-pagination
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/includes/admin/class-wc-admin-assets.php
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-items.php
- plugins/woocommerce/includes/class-wc-ajax.php
- plugins/woocommerce/tests/php/includes/class-wc-ajax-test.php

### #64626 [Sandbox] Order edit page UI explorations (not for review/merge)
https://github.com/woocommerce/woocommerce/pull/64626

Score: 5
Author: janamw27
Source search: All recent Woo PR activity: updated:>=2026-08-11
Why it matched: path: plugins/woocommerce/includes/admin; keyword: experiment; keyword: order edit
Touched areas:
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/client/legacy/js/admin/wc-enhanced-select.js
- plugins/woocommerce/includes/admin/meta-boxes/class-wc-meta-box-order-actions.php
- plugins/woocommerce/includes/admin/meta-boxes/class-wc-meta-box-order-data.php
- plugins/woocommerce/src/Internal/Admin/Orders/Edit.php

### #64482 Add Playwright e2e coverage for BIS alpha
https://github.com/woocommerce/woocommerce/pull/64482

Score: 4
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-08-11
Why it matched: keyword: rsm; keyword: stock notification
Touched areas:
- .markdownlintignore
- plugins/woocommerce/.wp-env.json
- plugins/woocommerce/changelog/rsm-437-bis-playwright-coverage
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/tests/e2e-pw/bin/bis-test-helpers.php
- plugins/woocommerce/tests/e2e-pw/bin/test-env-setup.sh
- plugins/woocommerce/tests/e2e-pw/tests/back-in-stock-notifications/README.md
- plugins/woocommerce/tests/e2e-pw/tests/back-in-stock-notifications/managing-notifications.spec.ts

### #64464 Flatten variable-product BIS signup to a real accessible form (RSM-446)
https://github.com/woocommerce/woocommerce/pull/64464

Score: 4
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-08-11
Why it matched: keyword: rsm; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/rsm-446-bis-variations-a11y
- plugins/woocommerce/client/legacy/css/woocommerce.scss
- plugins/woocommerce/client/legacy/js/frontend/back-in-stock-form.js
- plugins/woocommerce/src/Internal/StockNotifications/Frontend/ProductPageIntegration.php
- plugins/woocommerce/templates/single-product/back-in-stock-form.php
- plugins/woocommerce/tests/e2e-pw/tests/back-in-stock-notifications/signing-up-variable.spec.ts
- plugins/woocommerce/tests/e2e-pw/utils/back-in-stock-notifications.ts

### #64289 Add experimental Edge Cache Support for cart, checkout and mini-cart blocks
https://github.com/woocommerce/woocommerce/pull/64289

Score: 4
Author: jbouganim
Source search: All recent Woo PR activity: updated:>=2026-08-11
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

### #65487 Fix tooltip accessibility: keyboard navigation, ARIA roles, and WCAG 1.4.13 compliance
https://github.com/woocommerce/woocommerce/pull/65487

Score: 3
Author: anuj-rathore24
Source search: All recent Woo PR activity: updated:>=2026-08-11
Why it matched: path: plugins/woocommerce/includes/admin; keyword: navigation
Touched areas:
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-product.js
- plugins/woocommerce/client/legacy/js/admin/woocommerce_admin.js
- plugins/woocommerce/client/legacy/js/jquery-tiptip/jquery.tipTip.js
- plugins/woocommerce/includes/admin/meta-boxes/class-wc-meta-box-order-downloads.php
- plugins/woocommerce/includes/gateways/bacs/class-wc-gateway-bacs.php
- plugins/woocommerce/includes/wc-core-functions.php
- plugins/woocommerce/src/Internal/Admin/Orders/Edit.php

## Surface ownership policy

### Products table
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #67369 Load DataViews 17.1.0 safely for the new Settings UI
Intent: feature-flag
Action: draft-pr
Designer review path: Products > All Products
Matched by: keyword: dataviews
Auto-merge: held; the bot should leave a draft PR for review.
- Product-list DataViews work is worth pulling forward, but feature-flagged UI changes should pause as a draft for review.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #67369 Load DataViews 17.1.0 safely for the new Settings UI
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
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
Woo PR: #67335 Canonicalize Settings UI values before rendering
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings; keyword: settings ui
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

### Woo admin navigation
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #65487 Fix tooltip accessibility: keyboard navigation, ARIA roles, and WCAG 1.4.13 compliance
Intent: bugfix
Action: self-merge
Designer review path: WooCommerce admin rail
Matched by: keyword: navigation
- Navigation changes touch the frame of the whole prototype, so feature-flagged UI shifts should pause for review.

## Patch adapters

### Products table: DataViews adapter
Status: planned
Matched Woo PR: #67369 Load DataViews 17.1.0 safely for the new Settings UI
Local target: client/dataviews-tables/products-list
Designer review path: Products > All Products
Matched by: keyword: dataviews
- Translate the Woo product-list DataViews surface into a Future Woo products-list bundle.
- Keep the adapter separate from the existing orders-list DataViews bundle until the Products page has its own smoke test.

## Designer review paths

- Products > All Products
- WooCommerce admin rail
- WooCommerce > Settings

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

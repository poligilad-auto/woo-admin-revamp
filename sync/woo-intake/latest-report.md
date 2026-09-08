# Future Woo intake report

Generated: 2026-09-08
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-09-01`.
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

### #67865 Remove card header actions and obsolete styles from the Settings UI
https://github.com/woocommerce/woocommerce/pull/67865

Score: 12
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-01
Why it matched: keyword: dataviews; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment; keyword: navigation
Touched areas:
- packages/js/settings-ui/changelog/update-remove-group-actions
- packages/js/settings-ui/src/index.ts
- packages/js/settings-ui/src/registry.ts
- packages/js/settings-ui/src/types.ts
- plugins/woocommerce/changelog/dev-clean-settings-ui-styles
- plugins/woocommerce/changelog/dev-remove-settings-ui-group-actions
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/settings-ui.scss
- plugins/woocommerce/src/Internal/Admin/Settings/SettingsUISchema.php

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

### #68295 Add a pending-verification section to the Stock notifications My Account tab
https://github.com/woocommerce/woocommerce/pull/68295

Score: 8
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-09-01
Why it matched: keyword: feature flag; keyword: experiment; keyword: rsm; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/68292-my-account-pending-stock-notifications
- plugins/woocommerce/client/legacy/css/woocommerce.scss
- plugins/woocommerce/src/Internal/StockNotifications/Frontend/MyAccountEndpoint.php
- plugins/woocommerce/src/Internal/StockNotifications/Frontend/NotificationManagementService.php
- plugins/woocommerce/templates/myaccount/stock-notifications.php
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/my-account.spec.ts
- plugins/woocommerce/tests/php/src/Internal/StockNotifications/Frontend/MyAccountEndpointTests.php
- plugins/woocommerce/tests/php/src/Internal/StockNotifications/Frontend/NotificationManagementServiceTests.php

### #67864 Remove obsolete Settings UI styles
https://github.com/woocommerce/woocommerce/pull/67864

Score: 8
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-01
Why it matched: keyword: dataviews; keyword: settings-ui; keyword: settings ui; keyword: experiment
Touched areas:
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/README.md
- packages/js/settings-ui/changelog/fix-number-custom-attributes
- packages/js/settings-ui/changelog/fix-number-spin-control-scientific-precision
- packages/js/settings-ui/changelog/update-number-spin-control
- packages/js/settings-ui/changelog/update-remove-woo-field-renderers
- packages/js/settings-ui/changelog/update-wooprd-3596-dataform-renderer

### #66867 Restore WordPress defaults in the experimental Settings UI
https://github.com/woocommerce/woocommerce/pull/66867

Score: 8
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-01
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: experiment; keyword: navigation
Touched areas:
- packages/js/settings-ui/changelog/fix-preserve-wordpress-settings-behaviour
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/html-rendering.test.tsx
- packages/js/settings-ui/src/test/shell-header-visibility.test.tsx
- plugins/woocommerce/changelog/fix-settings-ui-shell-tab-focus-ring
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/settings-ui.scss

### #68408 Simplify Settings UI updates and preserve extension registrations
https://github.com/woocommerce/woocommerce/pull/68408

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-01
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: navigation
Touched areas:
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/changelog/fix-preserve-download-links
- packages/js/settings-ui/changelog/refactor-bounded-settings-ui-cleanup
- packages/js/settings-ui/changelog/refactor-settings-navigation-internals
- packages/js/settings-ui/src/dataform-adapter.tsx
- packages/js/settings-ui/src/registry.ts
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/dataform-adapter.test.tsx

### #67863 Remove Woo-owned Settings UI field renderers
https://github.com/woocommerce/woocommerce/pull/67863

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-01
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
Source search: All recent Woo PR activity: updated:>=2026-09-01
Why it matched: keyword: dataviews; keyword: settings-ui; keyword: settings ui
Touched areas:
- packages/js/settings-ui/changelog/add-wooprd-3595-dataform-adapter
- packages/js/settings-ui/src/dataform-adapter.tsx
- packages/js/settings-ui/src/html.ts
- packages/js/settings-ui/src/native-fields.tsx
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/dataform-adapter.test.tsx
- packages/js/settings-ui/src/values.ts

### #68464 Expose stock notifications settings through the REST settings API
https://github.com/woocommerce/woocommerce/pull/68464

Score: 4
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-09-01
Why it matched: keyword: feature flag; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/fix-wooplug-7691-stock-notifications-rest-settings
- plugins/woocommerce/src/Internal/StockNotifications/Admin/AdminManager.php
- plugins/woocommerce/src/Internal/StockNotifications/Admin/SettingsController.php
- plugins/woocommerce/src/Internal/StockNotifications/StockNotifications.php
- plugins/woocommerce/tests/php/src/Internal/StockNotifications/Admin/SettingsControllerTests.php
- plugins/woocommerce/tests/php/src/Internal/StockNotifications/StockNotificationsTests.php

### #68165 Fix Mini-Cart mutations aborted during navigation
https://github.com/woocommerce/woocommerce/pull/68165

Score: 4
Author: anandrajaram21
Source search: All recent Woo PR activity: updated:>=2026-09-01
Why it matched: keyword: experiment; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/68165-65956-mini-cart
- plugins/woocommerce/client/blocks/assets/js/base/stores/woocommerce/mutation-batcher.ts
- plugins/woocommerce/client/blocks/assets/js/base/stores/woocommerce/test/mutation-batcher.test.ts

### #67335 Canonicalize Settings UI values before rendering
https://github.com/woocommerce/woocommerce/pull/67335

Score: 4
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-09-01
Why it matched: keyword: settings-ui; keyword: settings ui
Touched areas:
- packages/js/settings-ui/changelog/fix-wooprd-3594-settings-value-boundary
- packages/js/settings-ui/package.json
- packages/js/settings-ui/src/dataform-adapter.tsx
- packages/js/settings-ui/src/hidden-inputs.tsx
- packages/js/settings-ui/src/registry.ts
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/dataform-adapter.test.tsx
- packages/js/settings-ui/src/test/hidden-inputs.test.ts

### #64439 Add My Account tab for Back in Stock Notifications (RSM-444)
https://github.com/woocommerce/woocommerce/pull/64439

Score: 4
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-09-01
Why it matched: keyword: rsm; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/64439-fix-stock-notifications-cancel-page
- plugins/woocommerce/changelog/64439-my-account-stock-notifications
- plugins/woocommerce/src/Internal/DataStores/StockNotifications/StockNotificationsDataStore.php
- plugins/woocommerce/src/Internal/StockNotifications/Frontend/MyAccountEndpoint.php
- plugins/woocommerce/src/Internal/StockNotifications/NotificationQuery.php
- plugins/woocommerce/src/Internal/StockNotifications/StockNotifications.php
- plugins/woocommerce/templates/myaccount/stock-notifications.php
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/my-account.spec.ts

### #67921 Fix negative quantity validation in the admin order editor
https://github.com/woocommerce/woocommerce/pull/67921

Score: 3
Author: ralucastan
Source search: All recent Woo PR activity: updated:>=2026-09-01
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit
Touched areas:
- plugins/woocommerce/changelog/fix-31068-order-item-qty-validation
- plugins/woocommerce/client/legacy/js/admin/backbone-modal.js
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-item.php
- plugins/woocommerce/includes/class-wc-ajax.php
- plugins/woocommerce/phpstan-baseline.neon
- plugins/woocommerce/src/Internal/Admin/Orders/ItemQuantityLimits.php
- plugins/woocommerce/tests/e2e/tests/order/order-item-quantity-validation.spec.ts

## Surface ownership policy

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #67865 Remove card header actions and obsolete styles from the Settings UI
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

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
Woo PR: #66867 Restore WordPress defaults in the experimental Settings UI
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #68408 Simplify Settings UI updates and preserve extension registrations
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
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

### Woo admin navigation
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #68165 Fix Mini-Cart mutations aborted during navigation
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce admin rail
Matched by: keyword: navigation
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

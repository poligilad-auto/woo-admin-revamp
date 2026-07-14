# Future Woo intake report

Generated: 2026-07-14
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-07-07`.
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

### #66437 Settings UI: shell header follows the page registration
https://github.com/woocommerce/woocommerce/pull/66437

Score: 10
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: navigation
Touched areas:
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/changelog/update-shell-header-top-level-pages
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/header-fields.test.tsx
- packages/js/settings-ui/src/test/html-rendering.test.tsx
- packages/js/settings-ui/src/test/shell-header-visibility.test.tsx
- packages/js/settings-ui/src/types.ts
- plugins/woocommerce/changelog/update-settings-ui-shell-header-top-level

### #65975 Add native Settings UI page provider for registered sections
https://github.com/woocommerce/woocommerce/pull/65975

Score: 10
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-07
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

### #64437 Add Stock Notifications analytics dashboard (RSM-445)
https://github.com/woocommerce/woocommerce/pull/64437

Score: 9
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: path: plugins/woocommerce/client/admin/client/analytics; keyword: experiment; keyword: rsm; keyword: analytics dashboard; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/rsm-445-bis-analytics-dashboard
- plugins/woocommerce/client/admin/client/analytics/report/notices/index.js
- plugins/woocommerce/client/admin/client/analytics/report/notices/style.scss
- plugins/woocommerce/client/admin/client/analytics/report/notices/use-notices-data.js
- plugins/woocommerce/client/admin/client/analytics/report/use-reports.js
- plugins/woocommerce/src/Internal/Admin/Analytics.php
- plugins/woocommerce/src/Internal/DataStores/StockNotifications/StockNotificationsDataStore.php
- plugins/woocommerce/src/Internal/StockNotifications/Admin/Analytics/RestController.php

### #66553 Fix Settings UI select trigger showing placeholder for empty-string option values
https://github.com/woocommerce/woocommerce/pull/66553

Score: 8
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment
Touched areas:
- packages/js/experimental-products-app/changelog/dev-correct-selectcontrol-comments
- packages/js/experimental-products-app/src/variation-view/fields/shipping_class/field.tsx
- packages/js/experimental-products-app/src/variation-view/fields/tax_class/field.tsx
- packages/js/settings-ui/changelog/fix-empty-string-option-trigger-label
- packages/js/settings-ui/src/native-fields.tsx
- packages/js/settings-ui/src/test/native-fields.test.tsx

### #64490 Move Back in Stock Notifications activation from wp-config flag to a Features setting
https://github.com/woocommerce/woocommerce/pull/64490

Score: 8
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: keyword: settings ui; keyword: feature flag; keyword: experiment; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/bis-features-screen-toggle
- plugins/woocommerce/includes/class-woocommerce.php
- plugins/woocommerce/src/Internal/DataStores/StockNotifications/StockNotificationsDataStore.php
- plugins/woocommerce/src/Internal/Features/FeaturesController.php
- plugins/woocommerce/tests/legacy/bootstrap.php

### #66561 [Settings UI] Fix value matching for extension-supplied schemas
https://github.com/woocommerce/woocommerce/pull/66561

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag
Touched areas:
- packages/js/settings-ui/changelog/fix-select-option-value-coercion
- packages/js/settings-ui/src/checkbox-values.ts
- packages/js/settings-ui/src/hidden-inputs.tsx
- packages/js/settings-ui/src/native-fields.tsx
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/header-fields.test.tsx
- packages/js/settings-ui/src/test/hidden-inputs.test.ts
- packages/js/settings-ui/src/test/html-rendering.test.tsx

### #66542 [Backport to release/11.0] Settings UI: adopt WPDS design tokens and components on settings pages
https://github.com/woocommerce/woocommerce/pull/66542

Score: 6
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag
Touched areas:
- .syncpackrc
- packages/js/settings-ui/changelog/update-adopt-wpds-components
- packages/js/settings-ui/src/native-fields.tsx
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/header-fields.test.tsx
- packages/js/settings-ui/src/types.ts
- plugins/woocommerce/changelog/update-settings-ui-wpds-token-delivery
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/index.tsx

### #66461 Settings UI: adopt WPDS design tokens and components on settings pages
https://github.com/woocommerce/woocommerce/pull/66461

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag
Touched areas:
- .syncpackrc
- packages/js/settings-ui/changelog/update-adopt-wpds-components
- packages/js/settings-ui/src/native-fields.tsx
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/header-fields.test.tsx
- packages/js/settings-ui/src/types.ts
- plugins/woocommerce/changelog/update-settings-ui-wpds-token-delivery
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/index.tsx

### #66456 [Backport to release/11.0] Render Settings UI cards with WordPress Design System components
https://github.com/woocommerce/woocommerce/pull/66456

Score: 6
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag
Touched areas:
- packages/js/settings-ui/changelog/add-wpds-shell-components
- packages/js/settings-ui/package.json
- packages/js/settings-ui/src/settings-ui-page.tsx
- plugins/woocommerce/changelog/update-settings-ui-wpds-cards
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/settings-ui.scss
- pnpm-lock.yaml
- pnpm-workspace.yaml

### #66403 Render Settings UI cards with WordPress Design System components
https://github.com/woocommerce/woocommerce/pull/66403

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag
Touched areas:
- packages/js/settings-ui/changelog/add-wpds-shell-components
- packages/js/settings-ui/package.json
- packages/js/settings-ui/src/settings-ui-page.tsx
- plugins/woocommerce/changelog/update-settings-ui-wpds-cards
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/settings-ui.scss
- pnpm-lock.yaml
- pnpm-workspace.yaml

### #66232 Keep Settings UI field values in the schema's value vocabulary
https://github.com/woocommerce/woocommerce/pull/66232

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-07
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

### #66039 Add search and pagination to order tax modal
https://github.com/woocommerce/woocommerce/pull/66039

Score: 5
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit; author: j111q
Touched areas:
- plugins/woocommerce/changelog/add-tax-rate-modal-search-pagination
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/includes/admin/class-wc-admin-assets.php
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-items.php
- plugins/woocommerce/includes/class-wc-ajax.php
- plugins/woocommerce/tests/php/includes/class-wc-ajax-test.php

### #65636 Add deprecated WC Admin feature flag shims
https://github.com/woocommerce/woocommerce/pull/65636

Score: 5
Author: gigitux
Source search: All recent Woo PR activity: updated:>=2026-07-07
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

### #66593 Document Settings UI native controls
https://github.com/woocommerce/woocommerce/pull/66593

Score: 4
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: keyword: settings-ui; keyword: settings ui
Touched areas:
- docs/extensions/settings-and-config/settings-ui.md

### #66487 Update Blocks feature flags and experimental interfaces docs
https://github.com/woocommerce/woocommerce/pull/66487

Score: 4
Author: gigitux
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: keyword: feature flag; keyword: experiment
Touched areas:
- plugins/woocommerce/client/blocks/docs/internal-developers/blocks/README.md
- plugins/woocommerce/client/blocks/docs/internal-developers/blocks/feature-flags-and-experimental-interfaces.md

### #66418 Fix false "unsaved changes"/"Leave site?" warning on the order edit screen
https://github.com/woocommerce/woocommerce/pull/66418

Score: 4
Author: towytowy
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: keyword: order edit; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/66418-fix-order-edit-unsaved-changes-warning
- plugins/woocommerce/changelog/fix-66308-order-edit-unsaved-changes-warning
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js

### #66110 Fix duplicate shipping marketplace link
https://github.com/woocommerce/woocommerce/pull/66110

Score: 4
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: path: plugins/woocommerce/client/admin/client/shipping; path: plugins/woocommerce/includes/admin; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/fix-duplicate-shipping-marketplace-link
- plugins/woocommerce/client/admin/client/hooks/test/use-endpoint-dismiss.test.ts
- plugins/woocommerce/client/admin/client/hooks/test/use-option-dismiss.test.ts
- plugins/woocommerce/client/admin/client/hooks/use-endpoint-dismiss.ts
- plugins/woocommerce/client/admin/client/hooks/use-option-dismiss.ts
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations-utils.tsx
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations.scss
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations.tsx

### #64439 Add My Account tab for Back in Stock Notifications (RSM-444)
https://github.com/woocommerce/woocommerce/pull/64439

Score: 4
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-07-07
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

### #64367 Rate-limit BIS sign-ups (RSM-441)
https://github.com/woocommerce/woocommerce/pull/64367

Score: 4
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: keyword: rsm; keyword: stock notification
Touched areas:
- plugins/woocommerce/.wp-env.json
- plugins/woocommerce/changelog/bis-alpha-cr-fixes-and-cleanup
- plugins/woocommerce/changelog/rsm-441-rate-limit-bis-signups
- plugins/woocommerce/phpstan-baseline.neon
- plugins/woocommerce/src/Internal/StockNotifications/Admin/NotificationEditPage.php
- plugins/woocommerce/src/Internal/StockNotifications/Admin/Templates/html-admin-notification-create.php
- plugins/woocommerce/src/Internal/StockNotifications/AsyncTasks/NotificationsProcessor.php
- plugins/woocommerce/src/Internal/StockNotifications/Config.php

### #66579 Fix order edit AJAX error and prevent `autosave.js` from loading on WC screens
https://github.com/woocommerce/woocommerce/pull/66579

Score: 3
Author: jorgeatorres
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit
Touched areas:
- plugins/woocommerce/changelog/66411-fix-order-edit-sample-permalink-403
- plugins/woocommerce/client/legacy/js/admin/woocommerce_admin.js
- plugins/woocommerce/includes/admin/class-wc-admin-assets.php
- plugins/woocommerce/tests/e2e/tests/order/order-edit.spec.ts
- plugins/woocommerce/tests/php/includes/admin/class-wc-admin-assets-test.php

### #66348 Add warnings for shadowed shipping zones
https://github.com/woocommerce/woocommerce/pull/66348

Score: 3
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-07-07
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
Source search: All recent Woo PR activity: updated:>=2026-07-07
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit
Touched areas:
- plugins/woocommerce/changelog/dsgwoo-1343-hide-downloads-metabox
- plugins/woocommerce/includes/admin/class-wc-admin-post-types.php
- plugins/woocommerce/phpstan-baseline.neon
- plugins/woocommerce/tests/e2e/tests/order/order-edit.spec.ts
- plugins/woocommerce/tests/unit-tests/admin/class-wc-tests-admin-post-types.php

## Surface ownership policy

### Analytics dashboard
Mode: vision-owned
Owner: Future Woo design
Woo PR: #64437 Add Stock Notifications analytics dashboard (RSM-445)
Intent: feature-flag
Action: draft-pr
Designer review path: Analytics
Matched by: path: plugins/woocommerce/client/admin/client/analytics; keyword: analytics dashboard; keyword: analytics
Auto-merge: held; the bot should leave a draft PR for review.
- Future Woo owns a super-future version of this surface, so Woo core changes stay visible without automatically overwriting it.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66437 Settings UI: shell header follows the page registration
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

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
Woo PR: #66553 Fix Settings UI select trigger showing placeholder for empty-string option values
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66561 [Settings UI] Fix value matching for extension-supplied schemas
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66542 [Backport to release/11.0] Settings UI: adopt WPDS design tokens and components on settings pages
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66461 Settings UI: adopt WPDS design tokens and components on settings pages
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66456 [Backport to release/11.0] Render Settings UI cards with WordPress Design System components
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66403 Render Settings UI cards with WordPress Design System components
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
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
Woo PR: #66593 Document Settings UI native controls
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
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
- Analytics
- WooCommerce > Settings
- WooCommerce > Settings > Shipping

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

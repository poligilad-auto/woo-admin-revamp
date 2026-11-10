# Future Woo intake report

Generated: 2026-11-10
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-11-03`.
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

### #66553 Fix Settings UI select trigger showing placeholder for empty-string option values
https://github.com/woocommerce/woocommerce/pull/66553

Score: 8
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-11-03
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment
Touched areas:
- packages/js/experimental-products-app/changelog/dev-correct-selectcontrol-comments
- packages/js/experimental-products-app/src/variation-view/fields/shipping_class/field.tsx
- packages/js/experimental-products-app/src/variation-view/fields/tax_class/field.tsx
- packages/js/settings-ui/changelog/fix-empty-string-option-trigger-label
- packages/js/settings-ui/src/native-fields.tsx
- packages/js/settings-ui/src/test/native-fields.test.tsx

### #64711 Add Newer / Older order navigation to the Order edit page header
https://github.com/woocommerce/woocommerce/pull/64711

Score: 6
Author: janamw27
Source search: All recent Woo PR activity: updated:>=2026-11-03
Why it matched: keyword: feature flag; keyword: order edit; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/order-detail-newer-older-nav
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/src/Internal/Admin/Orders/Edit.php
- plugins/woocommerce/src/Internal/Admin/Orders/OrderNavigation.php
- plugins/woocommerce/tests/php/src/Internal/Admin/Orders/OrderNavigationTest.php

### #70550 Allow decimal quantity for order items in the admin order editor
https://github.com/woocommerce/woocommerce/pull/70550

Score: 5
Author: anuj-rathore24
Source search: All recent Woo PR activity: updated:>=2026-11-03
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/fix-order-item-qty-step-validation
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-item.php
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-items.php
- plugins/woocommerce/includes/class-wc-ajax.php
- plugins/woocommerce/src/Internal/Admin/Orders/ItemQuantityLimits.php
- plugins/woocommerce/tests/e2e/tests/order/order-item-quantity-validation.spec.ts
- plugins/woocommerce/tests/php/includes/class-wc-ajax-test.php

### #70667 Add stock notification columns to the Analytics Stock report
https://github.com/woocommerce/woocommerce/pull/70667

Score: 4
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-11-03
Why it matched: path: plugins/woocommerce/client/admin/client/analytics; path: plugins/woocommerce/src/Admin; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/add-stock-report-notification-columns
- plugins/woocommerce/client/admin/client/analytics/report/stock/table.js
- plugins/woocommerce/src/Admin/API/Reports/Stock/Controller.php
- plugins/woocommerce/src/Internal/DataStores/StockNotifications/StockNotificationsDataStore.php
- plugins/woocommerce/src/Internal/StockNotifications/StockNotifications.php
- plugins/woocommerce/src/Internal/StockNotifications/StockReportColumns.php
- plugins/woocommerce/tests/php/src/Admin/API/Reports/Stock/ControllerTest.php

### #70328 Agent readiness: product and store checks behind a feature flag
https://github.com/woocommerce/woocommerce/pull/70328

Score: 4
Author: annamag
Source search: All recent Woo PR activity: updated:>=2026-11-03
Why it matched: keyword: feature flag; keyword: experiment
Touched areas:
- plugins/woocommerce/changelog/add-agent-readiness-status
- plugins/woocommerce/includes/class-woocommerce.php
- plugins/woocommerce/src/Internal/AgentReadiness/AgentReadiness.php
- plugins/woocommerce/src/Internal/AgentReadiness/Checks/AbstractReadinessCheck.php
- plugins/woocommerce/src/Internal/AgentReadiness/Checks/DuplicateGtinCheck.php
- plugins/woocommerce/src/Internal/AgentReadiness/Checks/ImageTooSmallCheck.php
- plugins/woocommerce/src/Internal/AgentReadiness/Checks/MissingBrandCheck.php
- plugins/woocommerce/src/Internal/AgentReadiness/Checks/MissingGtinCheck.php

### #69024 Add a Stock notifications report to Analytics
https://github.com/woocommerce/woocommerce/pull/69024

Score: 4
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-11-03
Why it matched: path: plugins/woocommerce/client/admin/client/analytics; path: plugins/woocommerce/src/Admin; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/add-wooplug-7570-stock-notifications-analytics-report
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/config.js
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/index.js
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/table.js
- plugins/woocommerce/client/admin/client/analytics/report/use-reports.js
- plugins/woocommerce/src/Admin/API/Init.php
- plugins/woocommerce/src/Admin/API/Reports/Export/Controller.php
- plugins/woocommerce/src/Admin/API/Reports/StatsDataStoreTrait.php

### #66593 Document Settings UI native controls
https://github.com/woocommerce/woocommerce/pull/66593

Score: 4
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-11-03
Why it matched: keyword: settings-ui; keyword: settings ui
Touched areas:
- docs/extensions/settings-and-config/settings-ui.md

### #69984 Bucket Stock notifications report intervals with per-row DST offsets
https://github.com/woocommerce/woocommerce/pull/69984

Score: 3
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-11-03
Why it matched: path: plugins/woocommerce/src/Admin; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/fix-stock-notifications-report-dst-buckets
- plugins/woocommerce/src/Admin/API/Reports/StockNotifications/DataStore.php
- plugins/woocommerce/src/Admin/API/Reports/StockNotifications/Stats/DataStore.php
- plugins/woocommerce/src/Admin/API/Reports/TimeInterval.php
- plugins/woocommerce/src/Internal/Admin/Reports/HposLegacyOrderReportQueryBuilder.php
- plugins/woocommerce/tests/php/src/Admin/API/Reports/StockNotifications/Stats/ControllerTest.php
- plugins/woocommerce/tests/php/src/Admin/API/Reports/TimeIntervalTest.php

## Surface ownership policy

### Analytics dashboard
Mode: vision-owned
Owner: Future Woo design
Woo PR: #70667 Add stock notification columns to the Analytics Stock report
Intent: default
Action: report-only
Designer review path: Analytics
Matched by: path: plugins/woocommerce/client/admin/client/analytics; keyword: analytics
Auto-apply: skipped; this stays visible without overwriting the Future Woo surface.
- Future Woo owns a super-future version of this surface, so Woo core changes stay visible without automatically overwriting it.

### Analytics dashboard
Mode: vision-owned
Owner: Future Woo design
Woo PR: #69024 Add a Stock notifications report to Analytics
Intent: default
Action: report-only
Designer review path: Analytics
Matched by: path: plugins/woocommerce/client/admin/client/analytics; keyword: analytics
Auto-apply: skipped; this stays visible without overwriting the Future Woo surface.
- Future Woo owns a super-future version of this surface, so Woo core changes stay visible without automatically overwriting it.

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
Woo PR: #66593 Document Settings UI native controls
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
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
Woo PR: #64711 Add Newer / Older order navigation to the Order edit page header
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
- Analytics
- WooCommerce > Settings

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

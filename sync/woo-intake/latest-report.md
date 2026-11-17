# Future Woo intake report

Generated: 2026-11-17
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-11-10`.
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

### #70923 Experiment: Add a Create shipping label box to the order edit screen
https://github.com/woocommerce/woocommerce/pull/70923

Score: 6
Author: bogdanungureanu
Source search: All recent Woo PR activity: updated:>=2026-11-10
Why it matched: path: plugins/woocommerce/client/admin/client/shipping; path: plugins/woocommerce/src/Admin; keyword: experiment; keyword: order edit
Touched areas:
- plugins/woocommerce/changelog/add-create-shipping-label-button
- plugins/woocommerce/client/admin/client/shipping/packlink-item.tsx
- plugins/woocommerce/client/admin/client/shipping/shipping-extension-item.tsx
- plugins/woocommerce/client/admin/client/shipping/shipping-extensions.ts
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations-marketplace-link.tsx
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations-utils.tsx
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations.tsx
- plugins/woocommerce/client/admin/client/shipping/shipstation-item.tsx

### #64711 Add Newer / Older order navigation to the Order edit page header
https://github.com/woocommerce/woocommerce/pull/64711

Score: 6
Author: janamw27
Source search: All recent Woo PR activity: updated:>=2026-11-10
Why it matched: keyword: feature flag; keyword: order edit; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/order-detail-newer-older-nav
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/src/Internal/Admin/Orders/Edit.php
- plugins/woocommerce/src/Internal/Admin/Orders/OrderNavigation.php
- plugins/woocommerce/tests/php/src/Internal/Admin/Orders/OrderNavigationTest.php

### #70667 Add stock notification columns to the Analytics Stock report
https://github.com/woocommerce/woocommerce/pull/70667

Score: 4
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-11-10
Why it matched: path: plugins/woocommerce/client/admin/client/analytics; path: plugins/woocommerce/src/Admin; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/add-stock-report-notification-columns
- plugins/woocommerce/client/admin/client/analytics/report/stock/table.js
- plugins/woocommerce/src/Admin/API/Reports/Stock/Controller.php
- plugins/woocommerce/src/Internal/DataStores/StockNotifications/StockNotificationsDataStore.php
- plugins/woocommerce/src/Internal/StockNotifications/StockNotifications.php
- plugins/woocommerce/src/Internal/StockNotifications/StockReportColumns.php
- plugins/woocommerce/tests/php/src/Admin/API/Reports/Stock/ControllerTest.php

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

### Shipping providers
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #70923 Experiment: Add a Create shipping label box to the order edit screen
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings > Shipping
Matched by: path: plugins/woocommerce/client/admin/client/shipping
Auto-merge: held; the bot should leave a draft PR for review.
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
- WooCommerce > Settings > Shipping

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

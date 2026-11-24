# Future Woo intake report

Generated: 2026-11-24
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-11-17`.
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

### #71365 Prototype: AI assistant experiments switch on the Features page
https://github.com/woocommerce/woocommerce/pull/71365

Score: 4
Author: poligilad-auto
Source search: All recent Woo PR activity: updated:>=2026-11-17
Why it matched: keyword: feature flag; keyword: experiment
Touched areas:
- plugins/woocommerce/changelog/add-ai-assistant-experiments-switch
- plugins/woocommerce/client/admin/client/sales-readiness/components/experiments-notice.tsx
- plugins/woocommerce/client/admin/client/sales-readiness/components/section-card.tsx
- plugins/woocommerce/client/admin/client/sales-readiness/index.tsx
- plugins/woocommerce/client/admin/client/sales-readiness/sales-readiness.scss
- plugins/woocommerce/client/admin/client/sales-readiness/test/section-card.test.tsx
- plugins/woocommerce/client/admin/client/sales-readiness/types.ts
- plugins/woocommerce/src/Internal/AgentReadiness/AiAssistantExperiments.php

### #70667 Add stock notification columns to the Analytics Stock report
https://github.com/woocommerce/woocommerce/pull/70667

Score: 4
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-11-17
Why it matched: path: plugins/woocommerce/client/admin/client/analytics; path: plugins/woocommerce/src/Admin; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/add-stock-report-notification-columns
- plugins/woocommerce/client/admin/client/analytics/report/stock/table.js
- plugins/woocommerce/src/Admin/API/Reports/Stock/Controller.php
- plugins/woocommerce/src/Internal/StockNotifications/StockNotifications.php
- plugins/woocommerce/src/Internal/StockNotifications/StockReportColumns.php
- plugins/woocommerce/tests/php/src/Admin/API/Reports/Stock/ControllerTest.php
- plugins/woocommerce/tests/php/src/Internal/StockNotifications/StockNotificationsFeatureTrait.php

### #69024 Add a Stock notifications report to Analytics
https://github.com/woocommerce/woocommerce/pull/69024

Score: 4
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-11-17
Why it matched: path: plugins/woocommerce/client/admin/client/analytics; path: plugins/woocommerce/src/Admin; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/add-wooplug-7570-stock-notifications-analytics-report
- plugins/woocommerce/client/admin/client/analytics/components/report-table/style.scss
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/config.js
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/index.js
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/table.js
- plugins/woocommerce/client/admin/client/analytics/report/use-reports.js
- plugins/woocommerce/src/Admin/API/Init.php
- plugins/woocommerce/src/Admin/API/Reports/Export/Controller.php

### #69984 Bucket Stock notifications report intervals with per-row DST offsets
https://github.com/woocommerce/woocommerce/pull/69984

Score: 3
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-11-17
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

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

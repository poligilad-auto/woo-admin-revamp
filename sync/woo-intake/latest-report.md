# Future Woo intake report

Generated: 2026-09-29
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-09-22`.
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

### #69173 Remove the experimental Settings UI JS
https://github.com/woocommerce/woocommerce/pull/69173

Score: 11
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-22
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

### #64437 Add Stock Notifications analytics dashboard (RSM-445)
https://github.com/woocommerce/woocommerce/pull/64437

Score: 9
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-09-22
Why it matched: path: plugins/woocommerce/client/admin/client/analytics; keyword: experiment; keyword: rsm; keyword: analytics dashboard; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/rsm-445-bis-analytics-dashboard
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/index.js
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/style.scss
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/test/use-stock-notifications-report-data.test.js
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/use-stock-notifications-report-data.js
- plugins/woocommerce/client/admin/client/analytics/report/use-reports.js
- plugins/woocommerce/src/Internal/Admin/Analytics.php
- plugins/woocommerce/src/Internal/DataStores/StockNotifications/StockNotificationsDataStore.php

### #69172 Deprecate the experimental Settings UI PHP classes
https://github.com/woocommerce/woocommerce/pull/69172

Score: 8
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-22
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

### #69174 Remove the Settings UI docs
https://github.com/woocommerce/woocommerce/pull/69174

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-22
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: experiment
Touched areas:
- docs/extensions/settings-and-config/extend-wc-settings-page.md
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md

### #69024 Add a Stock notifications report to Analytics
https://github.com/woocommerce/woocommerce/pull/69024

Score: 6
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-09-22
Why it matched: path: plugins/woocommerce/client/admin/client/analytics; path: plugins/woocommerce/src/Admin; keyword: feature flag; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/add-wooplug-7570-stock-notifications-analytics-report
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/config.js
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/index.js
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/table.js
- plugins/woocommerce/client/admin/client/analytics/report/use-reports.js
- plugins/woocommerce/src/Admin/API/Init.php
- plugins/woocommerce/src/Admin/API/Reports/StockNotifications/Controller.php
- plugins/woocommerce/src/Admin/API/Reports/StockNotifications/DataStore.php

### #69145 [Backport to release/11.2] Skip front-end stock notification services on admin requests
https://github.com/woocommerce/woocommerce/pull/69145

Score: 4
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-09-22
Why it matched: keyword: experiment; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/fix-WOOPLUG-5228-frontend-services
- plugins/woocommerce/src/Internal/StockNotifications/StockNotifications.php

### #69021 Skip front-end stock notification services on admin requests
https://github.com/woocommerce/woocommerce/pull/69021

Score: 4
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-09-22
Why it matched: keyword: experiment; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/fix-WOOPLUG-5228-frontend-services
- plugins/woocommerce/src/Internal/StockNotifications/StockNotifications.php

### #68989 Add an experimental cart recovery email and its settings
https://github.com/woocommerce/woocommerce/pull/68989

Score: 4
Author: ahmedevsaad
Source search: All recent Woo PR activity: updated:>=2026-09-22
Why it matched: keyword: feature flag; keyword: experiment
Touched areas:
- plugins/woocommerce/changelog/add-cart-recovery-email
- plugins/woocommerce/includes/class-wc-emails.php
- plugins/woocommerce/includes/emails/class-wc-email-customer-cart-recovery.php
- plugins/woocommerce/src/Internal/EmailEditor/WCTransactionalEmails/WCTransactionalEmails.php
- plugins/woocommerce/src/Internal/Features/FeaturesController.php
- plugins/woocommerce/templates/emails/block/customer-cart-recovery.php
- plugins/woocommerce/templates/emails/customer-cart-recovery.php
- plugins/woocommerce/templates/emails/plain/customer-cart-recovery.php

### #68986 Fix Screen Options fatal with Back in Stock Notifications
https://github.com/woocommerce/woocommerce/pull/68986

Score: 4
Author: oaratovskyi
Source search: All recent Woo PR activity: updated:>=2026-09-22
Why it matched: keyword: experiment; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/fix-stock-notifications-screen-options-fatal
- plugins/woocommerce/src/Internal/StockNotifications/Admin/MenusController.php
- plugins/woocommerce/tests/php/src/Internal/StockNotifications/Admin/MenusControllerTests.php

### #68851 Fix layout of the stock notification admin screens
https://github.com/woocommerce/woocommerce/pull/68851

Score: 4
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-09-22
Why it matched: keyword: order edit; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/fix-bis-notification-actions-apply-button
- plugins/woocommerce/client/legacy/css/admin.scss

### #68075 Analytics: add a setting to exclude free orders from report totals
https://github.com/woocommerce/woocommerce/pull/68075

Score: 4
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-09-22
Why it matched: path: plugins/woocommerce/client/admin/client/analytics; path: plugins/woocommerce/src/Admin; author: j111q
Touched areas:
- plugins/woocommerce/changelog/32194-analytics-exclude-free-orders
- plugins/woocommerce/client/admin/client/analytics/settings/config.js
- plugins/woocommerce/client/admin/client/analytics/settings/setting.scss
- plugins/woocommerce/src/Admin/API/Reports/Coupons/Stats/DataStore.php
- plugins/woocommerce/src/Admin/API/Reports/Customers/DataStore.php
- plugins/woocommerce/src/Admin/API/Reports/DataStore.php
- plugins/woocommerce/src/Admin/API/Reports/Orders/DataStore.php
- plugins/woocommerce/src/Admin/API/Reports/Orders/Stats/DataStore.php

### #69170 Add experimental block editor for product descriptions
https://github.com/woocommerce/woocommerce/pull/69170

Score: 3
Author: businessbloomer
Source search: All recent Woo PR activity: updated:>=2026-09-22
Why it matched: path: plugins/woocommerce/includes/admin; keyword: experiment
Touched areas:
- plugins/woocommerce/changelog/add-product-description-block-editor
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-product-variation.js
- plugins/woocommerce/client/legacy/js/admin/product-block-editor.js
- plugins/woocommerce/includes/admin/class-wc-admin-assets.php
- plugins/woocommerce/includes/admin/class-wc-admin-post-types.php
- plugins/woocommerce/includes/class-wc-post-types.php
- plugins/woocommerce/src/Internal/Features/FeaturesController.php
- plugins/woocommerce/tests/php/includes/admin/class-wc-admin-post-types-test.php

### #69062 Fix cleared shipping costs in order edits
https://github.com/woocommerce/woocommerce/pull/69062

Score: 3
Author: oaratovskyi
Source search: All recent Woo PR activity: updated:>=2026-09-22
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit
Touched areas:
- plugins/woocommerce/changelog/fix-44110-empty-shipping-cost
- plugins/woocommerce/includes/admin/wc-admin-functions.php
- plugins/woocommerce/tests/php/includes/admin/class-wc-admin-functions-test.php

### #68995 Reference branch for #68127 — ten metrics, grid columns, and a first-run tour
https://github.com/woocommerce/woocommerce/pull/68995

Score: 3
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-09-22
Why it matched: path: plugins/woocommerce/src/Admin; author: j111q
Touched areas:
- packages/js/components/changelog/68127-summary-grid-columns
- packages/js/components/src/summary/style.scss
- packages/js/components/src/summary/utils.js
- plugins/woocommerce/changelog/68127-analytics-metrics-reference
- plugins/woocommerce/changelog/wooa7s-1890-enable-performance-metrics-by-default
- plugins/woocommerce/client/admin/client/dashboard/default-sections.js
- plugins/woocommerce/client/admin/client/dashboard/store-performance/index.js
- plugins/woocommerce/src/Admin/API/Options.php

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

### Analytics dashboard
Mode: vision-owned
Owner: Future Woo design
Woo PR: #69024 Add a Stock notifications report to Analytics
Intent: feature-flag
Action: draft-pr
Designer review path: Analytics
Matched by: path: plugins/woocommerce/client/admin/client/analytics; keyword: analytics
Auto-merge: held; the bot should leave a draft PR for review.
- Future Woo owns a super-future version of this surface, so Woo core changes stay visible without automatically overwriting it.

### Analytics dashboard
Mode: vision-owned
Owner: Future Woo design
Woo PR: #68075 Analytics: add a setting to exclude free orders from report totals
Intent: default
Action: report-only
Designer review path: Analytics
Matched by: path: plugins/woocommerce/client/admin/client/analytics; keyword: analytics
Auto-apply: skipped; this stays visible without overwriting the Future Woo surface.
- Future Woo owns a super-future version of this surface, so Woo core changes stay visible without automatically overwriting it.

### Analytics dashboard
Mode: vision-owned
Owner: Future Woo design
Woo PR: #68995 Reference branch for #68127 — ten metrics, grid columns, and a first-run tour
Intent: vision-change
Action: self-merge
Designer review path: Analytics
Matched by: keyword: analytics
- Future Woo owns a super-future version of this surface, so Woo core changes stay visible without automatically overwriting it.

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
Woo PR: #69174 Remove the Settings UI docs
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
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
- Analytics
- WooCommerce > Settings

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

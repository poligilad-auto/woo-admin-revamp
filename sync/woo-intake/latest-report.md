# Future Woo intake report

Generated: 2026-10-06
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-09-29`.
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

### #67808 Add stock notification emails as WC_Email classes
https://github.com/woocommerce/woocommerce/pull/67808

Score: 7
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-09-29
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

### #69256 Fix Shop page field breaking the experimental Settings UI
https://github.com/woocommerce/woocommerce/pull/69256

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-29
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: experiment
Touched areas:
- plugins/woocommerce/changelog/fix-WOOAIRR-432-settings-ui-page-search
- plugins/woocommerce/src/Internal/Admin/Settings/SettingsUISchema.php
- plugins/woocommerce/tests/php/src/Internal/Admin/Settings/SettingsUISchemaTest.php

### #69151 Add an experimental payment settings screen scaffold
https://github.com/woocommerce/woocommerce/pull/69151

Score: 4
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-29
Why it matched: keyword: dataviews; keyword: experiment
Touched areas:
- plugins/woocommerce/.distignore
- plugins/woocommerce/.gitignore
- plugins/woocommerce/changelog/add-payment-settings-screen-scaffold
- plugins/woocommerce/client/admin/config/core.json
- plugins/woocommerce/client/admin/config/development.json
- plugins/woocommerce/eslint.config.mjs
- plugins/woocommerce/includes/class-woocommerce.php
- plugins/woocommerce/package.json

### #68075 Analytics: add a setting to exclude free orders from report totals
https://github.com/woocommerce/woocommerce/pull/68075

Score: 4
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-09-29
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

### #64289 Add experimental Edge Cache Support for cart, checkout and mini-cart blocks
https://github.com/woocommerce/woocommerce/pull/64289

Score: 4
Author: jbouganim
Source search: All recent Woo PR activity: updated:>=2026-09-29
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

## Surface ownership policy

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
Woo PR: #69256 Fix Shop page field breaking the experimental Settings UI
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

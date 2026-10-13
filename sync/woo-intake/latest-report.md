# Future Woo intake report

Generated: 2026-10-13
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-10-06`.
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

### #69663 Update the bundled DataViews package to 20.0.0
https://github.com/woocommerce/woocommerce/pull/69663

Score: 5
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-10-06
Why it matched: path: plugins/woocommerce/client/admin/client/settings; keyword: dataviews; keyword: experiment
Touched areas:
- packages/js/internal-js-tests/changelog/update-wp-bundled-dataviews-19
- packages/js/internal-js-tests/jest-preset.js
- plugins/woocommerce/changelog/update-wp-bundled-dataviews-19
- plugins/woocommerce/client/admin/client/settings-payments/offline/shipping-restriction-fields.tsx
- pnpm-lock.yaml
- pnpm-workspace.yaml

### #69151 Add an experimental payment settings screen scaffold
https://github.com/woocommerce/woocommerce/pull/69151

Score: 4
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-10-06
Why it matched: keyword: dataviews; keyword: experiment
Touched areas:
- plugins/woocommerce/.distignore
- plugins/woocommerce/admin-screens/.gitignore
- plugins/woocommerce/admin-screens/eslint.config.mjs
- plugins/woocommerce/admin-screens/package.json
- plugins/woocommerce/admin-screens/routes/payment-settings/package.json
- plugins/woocommerce/admin-screens/routes/payment-settings/stage.tsx
- plugins/woocommerce/admin-screens/tsconfig.json
- plugins/woocommerce/changelog/add-payment-settings-screen-scaffold

### #68801 Document the three site visibility states for integrators
https://github.com/woocommerce/woocommerce/pull/68801

Score: 4
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-10-06
Why it matched: keyword: feature flag; author: j111q
Touched areas:
- docs/extensions/extension-onboarding/integrating-coming-soon-mode.md

### #68075 Analytics: add a setting to exclude free orders from report totals
https://github.com/woocommerce/woocommerce/pull/68075

Score: 4
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-10-06
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
Source search: All recent Woo PR activity: updated:>=2026-10-06
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

### #68995 Reference branch for #68127 — ten metrics, grid columns, and a first-run tour
https://github.com/woocommerce/woocommerce/pull/68995

Score: 3
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-10-06
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

### Products table
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #69663 Update the bundled DataViews package to 20.0.0
Intent: feature-flag
Action: draft-pr
Designer review path: Products > All Products
Matched by: keyword: dataviews
Auto-merge: held; the bot should leave a draft PR for review.
- Product-list DataViews work is worth pulling forward, but feature-flagged UI changes should pause as a draft for review.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #69663 Update the bundled DataViews package to 20.0.0
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/client/admin/client/settings
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

### Products table: DataViews adapter
Status: planned
Matched Woo PR: #69663 Update the bundled DataViews package to 20.0.0
Local target: client/dataviews-tables/products-list
Designer review path: Products > All Products
Matched by: keyword: dataviews
- Translate the Woo product-list DataViews surface into a Future Woo products-list bundle.
- Keep the adapter separate from the existing orders-list DataViews bundle until the Products page has its own smoke test.

## Designer review paths

- Products > All Products
- WooCommerce admin rail
- Analytics
- WooCommerce > Settings

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

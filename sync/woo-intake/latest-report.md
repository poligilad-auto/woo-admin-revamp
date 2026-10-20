# Future Woo intake report

Generated: 2026-10-20
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-10-13`.
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

### #69024 Add a Stock notifications report to Analytics
https://github.com/woocommerce/woocommerce/pull/69024

Score: 6
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-10-13
Why it matched: path: plugins/woocommerce/client/admin/client/analytics; path: plugins/woocommerce/src/Admin; keyword: feature flag; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/add-wooplug-7570-stock-notifications-analytics-report
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/config.js
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/index.js
- plugins/woocommerce/client/admin/client/analytics/report/stock-notifications/table.js
- plugins/woocommerce/client/admin/client/analytics/report/use-reports.js
- plugins/woocommerce/phpstan-baseline.neon
- plugins/woocommerce/src/Admin/API/Init.php
- plugins/woocommerce/src/Admin/API/Reports/StatsDataStoreTrait.php

### #68545 WIP: Settings UI - Switch to opt-out by default
https://github.com/woocommerce/woocommerce/pull/68545

Score: 6
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-10-13
Why it matched: path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui
Touched areas:
- docs/extensions/settings-and-config/extend-wc-settings-page.md
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/README.md
- packages/js/settings-ui/src/dataform-adapter.tsx
- packages/js/settings-ui/src/hidden-inputs.tsx
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/dataform-adapter.test.tsx

### #64289 Add experimental Edge Cache Support for cart, checkout and mini-cart blocks
https://github.com/woocommerce/woocommerce/pull/64289

Score: 4
Author: jbouganim
Source search: All recent Woo PR activity: updated:>=2026-10-13
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

### #70013 [Backport to release/11.3] Show marketing channels to site admins on multisite
https://github.com/woocommerce/woocommerce/pull/70013

Score: 3
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-10-13
Why it matched: path: plugins/woocommerce/client/admin/client/marketing; keyword: marketing channels
Touched areas:
- plugins/woocommerce/changelog/55130-marketing-channels-multisite-site-admin
- plugins/woocommerce/client/admin/client/marketing/hooks/useRecommendedChannels.ts
- plugins/woocommerce/src/Internal/Admin/Marketing.php

### #69993 Show marketing channels to site admins on multisite
https://github.com/woocommerce/woocommerce/pull/69993

Score: 3
Author: yuliyan
Source search: All recent Woo PR activity: updated:>=2026-10-13
Why it matched: path: plugins/woocommerce/client/admin/client/marketing; keyword: marketing channels
Touched areas:
- plugins/woocommerce/changelog/55130-marketing-channels-multisite-site-admin
- plugins/woocommerce/client/admin/client/marketing/hooks/useRecommendedChannels.ts
- plugins/woocommerce/src/Internal/Admin/Marketing.php

### #69984 Bucket Stock notifications report intervals with per-row DST offsets
https://github.com/woocommerce/woocommerce/pull/69984

Score: 3
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-10-13
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
Woo PR: #69024 Add a Stock notifications report to Analytics
Intent: feature-flag
Action: draft-pr
Designer review path: Analytics
Matched by: path: plugins/woocommerce/client/admin/client/analytics; keyword: analytics
Auto-merge: held; the bot should leave a draft PR for review.
- Future Woo owns a super-future version of this surface, so Woo core changes stay visible without automatically overwriting it.

### Marketing and sales channels
Mode: vision-owned
Owner: Future Woo design
Woo PR: #70013 [Backport to release/11.3] Show marketing channels to site admins on multisite
Intent: default
Action: report-only
Designer review path: Marketing > Campaigns
Matched by: path: plugins/woocommerce/client/admin/client/marketing; keyword: marketing channels
Auto-apply: skipped; this stays visible without overwriting the Future Woo surface.
- Protects the future-facing Marketing > Campaigns exploration while still surfacing useful Woo changes.

### Marketing and sales channels
Mode: vision-owned
Owner: Future Woo design
Woo PR: #69993 Show marketing channels to site admins on multisite
Intent: bugfix
Action: report-only
Designer review path: Marketing > Campaigns
Matched by: path: plugins/woocommerce/client/admin/client/marketing; keyword: marketing channels
Auto-apply: skipped; this stays visible without overwriting the Future Woo surface.
- Protects the future-facing Marketing > Campaigns exploration while still surfacing useful Woo changes.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #68545 WIP: Settings UI - Switch to opt-out by default
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings; keyword: settings-ui; keyword: settings ui
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
- Marketing > Campaigns
- WooCommerce > Settings

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

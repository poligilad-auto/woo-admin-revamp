# Future Woo intake report

Generated: 2026-09-22
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-09-15`.
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

### #67334 Validate Settings UI schemas before rendering
https://github.com/woocommerce/woocommerce/pull/67334

Score: 8
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-09-15
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

### #68545 WIP: Settings UI - Switch to opt-out by default
https://github.com/woocommerce/woocommerce/pull/68545

Score: 6
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-09-15
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

### #68851 Fix layout of the stock notification admin screens
https://github.com/woocommerce/woocommerce/pull/68851

Score: 4
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-09-15
Why it matched: keyword: order edit; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/fix-bis-notification-actions-apply-button
- plugins/woocommerce/client/legacy/css/admin.scss

### #68800 Rename "Site visibility" settings tab to "Store visibility"
https://github.com/woocommerce/woocommerce/pull/68800

Score: 4
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-09-15
Why it matched: path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; author: j111q
Touched areas:
- plugins/woocommerce/changelog/dotsite-55-store-visibility-rename
- plugins/woocommerce/client/admin/client/blueprint/components/BlueprintUploadDropzone.tsx
- plugins/woocommerce/client/admin/client/blueprint/components/get-option-groups.ts
- plugins/woocommerce/client/admin/client/launch-your-store/hub/sidebar/components/launch-store-hub.tsx
- plugins/woocommerce/client/admin/client/launch-your-store/settings/components/confirmation-modal.jsx
- plugins/woocommerce/client/admin/client/launch-your-store/settings/slotfill.js
- plugins/woocommerce/includes/admin/settings/class-wc-settings-site-visibility.php
- plugins/woocommerce/src/Admin/Features/Blueprint/Exporters/ExportWCSettingsSiteVisibility.php

### #68737 [Backport to release/11.2] Enable BIS feature flag per E2E spec instead of env-wide
https://github.com/woocommerce/woocommerce/pull/68737

Score: 4
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-09-15
Why it matched: keyword: feature flag; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/68515-fix-bis-new-install-allow-signups
- plugins/woocommerce/includes/class-wc-install.php
- plugins/woocommerce/tests/e2e/bin/test-env-setup.sh
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/README.md
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/feature-disabled.spec.ts
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/managing-notifications.spec.ts
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/my-account.spec.ts
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/receiving-confirmations.spec.ts

### #68515 Enable BIS feature flag per E2E spec instead of env-wide
https://github.com/woocommerce/woocommerce/pull/68515

Score: 4
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-09-15
Why it matched: keyword: feature flag; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/68515-fix-bis-new-install-allow-signups
- plugins/woocommerce/includes/class-wc-install.php
- plugins/woocommerce/tests/e2e/bin/test-env-setup.sh
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/README.md
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/feature-disabled.spec.ts
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/managing-notifications.spec.ts
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/my-account.spec.ts
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/receiving-confirmations.spec.ts

### #64367 Rate-limit BIS sign-ups (RSM-441)
https://github.com/woocommerce/woocommerce/pull/64367

Score: 4
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-09-15
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

## Surface ownership policy

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
Woo PR: #68545 WIP: Settings UI - Switch to opt-out by default
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings; keyword: settings-ui; keyword: settings ui
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #68800 Rename "Site visibility" settings tab to "Store visibility"
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings
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
- WooCommerce > Settings

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

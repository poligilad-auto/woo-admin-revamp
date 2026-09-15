# Future Woo intake report

Generated: 2026-09-15
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-09-08`.
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

### #68498 Fix the Settings > Emails listing styles by loading the listing on demand
https://github.com/woocommerce/woocommerce/pull/68498

Score: 12
Author: costasovo
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: path: plugins/woocommerce/client/admin/client/settings; path: plugins/woocommerce/includes/admin; keyword: dataviews; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment
Touched areas:
- plugins/woocommerce/changelog/fix-email-listing-dataviews-styles
- plugins/woocommerce/client/admin/client/settings-email/__tests__/settings-email-listing-slotfill-load-error.test.tsx
- plugins/woocommerce/client/admin/client/settings-email/__tests__/settings-email-listing-slotfill.test.tsx
- plugins/woocommerce/client/admin/client/settings-email/settings-email-listing-data.ts
- plugins/woocommerce/client/admin/client/settings-email/settings-email-listing-rtl.scss
- plugins/woocommerce/client/admin/client/settings-email/settings-email-listing-slotfill.tsx
- plugins/woocommerce/client/admin/client/settings-email/settings-email-listing.scss
- plugins/woocommerce/client/admin/client/settings-email/style.scss

### #64712 Add nested admin navigation behind navigation_v2 feature flag
https://github.com/woocommerce/woocommerce/pull/64712

Score: 12
Author: beaulebens
Source search: All recent Woo PR activity: updated:>=2026-09-08; Tracked PR: Nested admin navigation
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
Source search: All recent Woo PR activity: updated:>=2026-09-08
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

### #65893 [Backport to release/10.9] Rename @woocommerce/settings-ui-sdk to @woocommerce/settings-ui
https://github.com/woocommerce/woocommerce/pull/65893

Score: 8
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: path: plugins/woocommerce/client/admin/client/settings; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: feature flag
Touched areas:
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/dependency-extraction-webpack-plugin/assets/packages.js
- packages/js/dependency-extraction-webpack-plugin/changelog/update-rename-settings-ui-entry
- packages/js/settings-ui-sdk/changelog/add-settings-ui-sdk
- packages/js/settings-ui-sdk/changelog/tweak-settings-ui-card-design
- packages/js/settings-ui/README.md
- packages/js/settings-ui/build.mjs

### #65729 [Backport to release/10.9] Align settings UI layout and number inputs with design spec
https://github.com/woocommerce/woocommerce/pull/65729

Score: 8
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment
Touched areas:
- packages/js/settings-ui-sdk/changelog/update-number-spin-control
- packages/js/settings-ui-sdk/package.json
- packages/js/settings-ui-sdk/src/native-fields.tsx
- packages/js/settings-ui-sdk/src/number-spin-control.tsx
- packages/js/settings-ui-sdk/src/test/native-fields.test.tsx
- plugins/woocommerce/changelog/update-settings-ui-layout-width-spacing
- plugins/woocommerce/changelog/update-settings-ui-number-spin-control-styles
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/settings-ui.scss

### #65719 Rename @woocommerce/settings-ui-sdk to @woocommerce/settings-ui
https://github.com/woocommerce/woocommerce/pull/65719

Score: 8
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: path: plugins/woocommerce/client/admin/client/settings; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: feature flag
Touched areas:
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/dependency-extraction-webpack-plugin/assets/packages.js
- packages/js/dependency-extraction-webpack-plugin/changelog/update-rename-settings-ui-entry
- packages/js/settings-ui-sdk/changelog/add-settings-ui-sdk
- packages/js/settings-ui-sdk/changelog/tweak-settings-ui-card-design
- packages/js/settings-ui/README.md
- packages/js/settings-ui/build.mjs

### #65695 Align settings UI layout and number inputs with design spec
https://github.com/woocommerce/woocommerce/pull/65695

Score: 8
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment
Touched areas:
- packages/js/settings-ui-sdk/changelog/update-number-spin-control
- packages/js/settings-ui-sdk/package.json
- packages/js/settings-ui-sdk/src/native-fields.tsx
- packages/js/settings-ui-sdk/src/number-spin-control.tsx
- packages/js/settings-ui-sdk/src/test/native-fields.test.tsx
- plugins/woocommerce/changelog/update-settings-ui-layout-width-spacing
- plugins/woocommerce/changelog/update-settings-ui-number-spin-control-styles
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/settings-ui.scss

### #68684 [tests] Stop the Settings UI E2E spec from corrupting wp-env's cache
https://github.com/woocommerce/woocommerce/pull/68684

Score: 6
Author: vladolaru
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag
Touched areas:
- plugins/woocommerce/changelog/fix-e2e-wp-env-cli-cache-race
- plugins/woocommerce/tests/e2e/README.md
- plugins/woocommerce/tests/e2e/tests/settings/settings-ui-feature-flag.spec.ts
- plugins/woocommerce/tests/e2e/utils/cli.ts

### #68545 WIP: Settings UI - Switch to opt-out by default
https://github.com/woocommerce/woocommerce/pull/68545

Score: 6
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-09-08
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

### #68408 Simplify Settings UI updates and preserve extension registrations
https://github.com/woocommerce/woocommerce/pull/68408

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-09-08
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

### #65130 Add experimental dashboard widgets framework with a Store Activity widget
https://github.com/woocommerce/woocommerce/pull/65130

Score: 6
Author: retrofox
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: dataviews; keyword: feature flag; keyword: experiment
Touched areas:
- .syncpackrc
- plugins/woocommerce/.gitignore
- plugins/woocommerce/changelog/add-dashboard-widgets-scaffold
- plugins/woocommerce/package.json
- plugins/woocommerce/packages/README.md
- plugins/woocommerce/packages/core-dashboard-init/README.md
- plugins/woocommerce/packages/core-dashboard-init/package.json
- plugins/woocommerce/packages/core-dashboard-init/src/data/constants.ts

### #65114 Polish the variations DataViews table and unify the stock pill
https://github.com/woocommerce/woocommerce/pull/65114

Score: 6
Author: poligilad-auto
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: dataviews; keyword: feature flag; keyword: experiment
Touched areas:
- packages/js/experimental-products-app/changelog/variations-dataviews-polish
- packages/js/experimental-products-app/src/fields/stock/field.test.tsx
- packages/js/experimental-products-app/src/fields/stock/field.tsx
- packages/js/experimental-products-app/src/product-edit/index.tsx
- packages/js/experimental-products-app/src/product-edit/utils.test.ts
- packages/js/experimental-products-app/src/variation-view/constants.ts
- packages/js/experimental-products-app/src/variation-view/fields.tsx
- packages/js/experimental-products-app/src/variation-view/index.tsx

### #64711 Add prev/next order navigation to Order detail page header
https://github.com/woocommerce/woocommerce/pull/64711

Score: 6
Author: janamw27
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: feature flag; keyword: order edit; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/order-detail-redesign-prev-next-nav
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/src/Internal/Admin/Orders/Edit.php
- plugins/woocommerce/src/Internal/Features/OrderDetailRedesign/OrderListNav.php
- plugins/woocommerce/tests/php/src/Internal/Features/OrderDetailRedesign/OrderListNavTest.php

### #64329 Apply CodeRabbit review fixes to Back in Stock Notifications alpha
https://github.com/woocommerce/woocommerce/pull/64329

Score: 6
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: rsm; keyword: stock notification; keyword: email template
Touched areas:
- .markdownlintignore
- plugins/woocommerce/changelog/bis-alpha-cr-fixes-and-cleanup
- plugins/woocommerce/phpstan-baseline.neon
- plugins/woocommerce/src/Internal/StockNotifications/Admin/NotificationEditPage.php
- plugins/woocommerce/src/Internal/StockNotifications/Admin/Templates/html-admin-notification-create.php
- plugins/woocommerce/src/Internal/StockNotifications/AsyncTasks/NotificationsProcessor.php
- plugins/woocommerce/src/Internal/StockNotifications/Config.php
- plugins/woocommerce/src/Internal/StockNotifications/DataRetentionController.php

### #64243 [DataViews - All Products] Clean up code
https://github.com/woocommerce/woocommerce/pull/64243

Score: 6
Author: gigitux
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: dataviews; keyword: experiment; keyword: navigation
Touched areas:
- packages/js/experimental-products-app/package.json
- packages/js/experimental-products-app/src/layout.tsx
- packages/js/experimental-products-app/src/product-edit/index.tsx
- packages/js/experimental-products-app/src/product-edit/style.scss
- packages/js/experimental-products-app/src/product-list/index.tsx
- packages/js/experimental-products-app/src/router.tsx
- packages/js/experimental-products-app/src/sidebar-dataviews/dataview-item.tsx
- packages/js/experimental-products-app/src/sidebar-dataviews/default-views.ts

### #65636 Add deprecated WC Admin feature flag shims
https://github.com/woocommerce/woocommerce/pull/65636

Score: 5
Author: gigitux
Source search: All recent Woo PR activity: updated:>=2026-09-08
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

### #64184 [Experimental] Create @woocommerce/experimental-products-app package (#64182)
https://github.com/woocommerce/woocommerce/pull/64184

Score: 5
Author: gigitux
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: path: plugins/woocommerce/src/Admin; keyword: dataviews; keyword: experiment
Touched areas:
- .syncpackrc
- packages/js/dependency-extraction-webpack-plugin/assets/packages.js
- packages/js/experimental-products-app/.eslintrc.js
- packages/js/experimental-products-app/.npmrc
- packages/js/experimental-products-app/babel.config.js
- packages/js/experimental-products-app/jest.config.json
- packages/js/experimental-products-app/package.json
- packages/js/experimental-products-app/src/app.tsx

### #64182 Create @woocommerce/experimental-products-app package
https://github.com/woocommerce/woocommerce/pull/64182

Score: 5
Author: gigitux
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: path: plugins/woocommerce/src/Admin; keyword: experiment; keyword: navigation
Touched areas:
- .syncpackrc
- packages/js/dependency-extraction-webpack-plugin/assets/packages.js
- packages/js/experimental-products-app/.eslintrc.js
- packages/js/experimental-products-app/.npmrc
- packages/js/experimental-products-app/babel.config.js
- packages/js/experimental-products-app/jest.config.json
- packages/js/experimental-products-app/package.json
- packages/js/experimental-products-app/src/app.tsx

### #68737 [Backport to release/11.2] Enable BIS feature flag per E2E spec instead of env-wide
https://github.com/woocommerce/woocommerce/pull/68737

Score: 4
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-09-08
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
Source search: All recent Woo PR activity: updated:>=2026-09-08
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

### #68464 Expose stock notifications settings through the REST settings API
https://github.com/woocommerce/woocommerce/pull/68464

Score: 4
Author: xristos3490
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: feature flag; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/fix-wooplug-7691-stock-notifications-rest-settings
- plugins/woocommerce/src/Internal/StockNotifications/Admin/AdminManager.php
- plugins/woocommerce/src/Internal/StockNotifications/Admin/SettingsController.php
- plugins/woocommerce/src/Internal/StockNotifications/StockNotifications.php
- plugins/woocommerce/tests/php/src/Internal/StockNotifications/Admin/SettingsControllerTests.php
- plugins/woocommerce/tests/php/src/Internal/StockNotifications/StockNotificationsTests.php

### #65521 Make abandoned cart recovery experimental and opt-in (not default-on for new installs)
https://github.com/woocommerce/woocommerce/pull/65521

Score: 4
Author: prettyboymp
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: feature flag; keyword: experiment
Touched areas:
- plugins/woocommerce/changelog/abandoned-cart-recovery-experimental-optin
- plugins/woocommerce/includes/class-wc-install.php
- plugins/woocommerce/src/Internal/Features/FeaturesController.php

### #65404 Remove `experimental-iapi-runtime` feature flag
https://github.com/woocommerce/woocommerce/pull/65404

Score: 4
Author: gigitux
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: feature flag; keyword: experiment
Touched areas:
- .pnpmfile.cjs
- .syncpackrc
- plugins/woocommerce/changelog/dev-remove-experimental-iapi-runtime
- plugins/woocommerce/client/admin/config/core.json
- plugins/woocommerce/client/admin/config/development.json
- plugins/woocommerce/client/blocks/assets/js/blocks/product-filters/frontend.ts
- plugins/woocommerce/client/blocks/bin/webpack-config-interactivity.js
- plugins/woocommerce/client/blocks/package.json

### #64727 Clear stock notification dedup meta on stock recovery
https://github.com/woocommerce/woocommerce/pull/64727

Score: 4
Author: adamgrzybkowski
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: rsm; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/issue-RSM-2345
- plugins/woocommerce/src/Internal/PushNotifications/PushNotifications.php
- plugins/woocommerce/src/Internal/PushNotifications/Triggers/StockNotificationRecoveryHandler.php
- plugins/woocommerce/tests/php/src/Internal/PushNotifications/Triggers/StockNotificationRecoveryHandlerTest.php

### #64700 Gate "saved for later" behind feature flag
https://github.com/woocommerce/woocommerce/pull/64700

Score: 4
Author: jorgeatorres
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: feature flag; keyword: experiment
Touched areas:
- plugins/woocommerce/changelog/add-shopper-collections-feature-flag
- plugins/woocommerce/src/Blocks/BlockTypes/Cart.php
- plugins/woocommerce/src/Blocks/BlockTypesController.php
- plugins/woocommerce/src/Internal/Features/FeaturesController.php
- plugins/woocommerce/src/StoreApi/RoutesController.php
- plugins/woocommerce/tests/php/src/Blocks/StoreApi/Routes/ShopperLists.php

### #64600 Add store_stock push notification for low/out/backorder events
https://github.com/woocommerce/woocommerce/pull/64600

Score: 4
Author: adamgrzybkowski
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: rsm; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/issue-RSM-1551
- plugins/woocommerce/src/Internal/PushNotifications/Controllers/NotificationPreferencesRestController.php
- plugins/woocommerce/src/Internal/PushNotifications/Notifications/Notification.php
- plugins/woocommerce/src/Internal/PushNotifications/Notifications/StockNotification.php
- plugins/woocommerce/src/Internal/PushNotifications/PushNotifications.php
- plugins/woocommerce/src/Internal/PushNotifications/Services/NotificationPreferencesService.php
- plugins/woocommerce/src/Internal/PushNotifications/Services/NotificationProcessor.php
- plugins/woocommerce/src/Internal/PushNotifications/Services/PendingNotificationStore.php

### #64497 [Email Editor] Add selective apply for block email template updates
https://github.com/woocommerce/woocommerce/pull/64497

Score: 4
Author: triple0t
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: rsm; keyword: email template
Touched areas:
- plugins/woocommerce/changelog/rsm-143-selective-apply
- plugins/woocommerce/changelog/rsm-143-selective-apply-drawer
- plugins/woocommerce/client/admin/client/wp-admin-scripts/email-editor-integration/hooks/use-apply-update.ts
- plugins/woocommerce/client/admin/client/wp-admin-scripts/email-editor-integration/hooks/use-change-summary.ts
- plugins/woocommerce/client/admin/client/wp-admin-scripts/email-editor-integration/index.ts
- plugins/woocommerce/client/admin/client/wp-admin-scripts/email-editor-integration/reset-notification-email-content.tsx
- plugins/woocommerce/client/admin/client/wp-admin-scripts/email-editor-integration/review-drawer.tsx
- plugins/woocommerce/client/admin/client/wp-admin-scripts/email-editor-integration/review-update-plugin.tsx

### #64482 Add Playwright e2e coverage for BIS alpha
https://github.com/woocommerce/woocommerce/pull/64482

Score: 4
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: rsm; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/rsm-437-bis-notification-image-overflow
- plugins/woocommerce/changelog/rsm-437-bis-playwright-coverage
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/tests/e2e/README.md
- plugins/woocommerce/tests/e2e/bin/test-env-setup.sh
- plugins/woocommerce/tests/e2e/playwright.config.ts
- plugins/woocommerce/tests/e2e/test-plugins/woocommerce-e2e-test-helper/woocommerce-e2e-test-helper.php
- plugins/woocommerce/tests/e2e/tests/back-in-stock-notifications/README.md

### #64439 Add My Account tab for Back in Stock Notifications (RSM-444)
https://github.com/woocommerce/woocommerce/pull/64439

Score: 4
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-09-08
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

### #64352 Add Playwright e2e coverage for BIS alpha
https://github.com/woocommerce/woocommerce/pull/64352

Score: 4
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: rsm; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/bis-alpha-cr-fixes-and-cleanup
- plugins/woocommerce/src/Internal/StockNotifications/CODERABBIT-TRIAGE-RAW.md
- plugins/woocommerce/src/Internal/StockNotifications/CODERABBIT-TRIAGE.md
- plugins/woocommerce/src/Internal/StockNotifications/SPRINT.md

### #64351 Add per-user push notification preferences
https://github.com/woocommerce/woocommerce/pull/64351

Score: 4
Author: adamgrzybkowski
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: feature flag; keyword: rsm
Touched areas:
- plugins/woocommerce/changelog/64351-issue-RSM-693
- plugins/woocommerce/src/Internal/PushNotifications/Controllers/NotificationPreferencesRestController.php
- plugins/woocommerce/src/Internal/PushNotifications/Controllers/PushTokenRestController.php
- plugins/woocommerce/src/Internal/PushNotifications/DataStores/NotificationPreferencesDataStore.php
- plugins/woocommerce/src/Internal/PushNotifications/PushNotifications.php
- plugins/woocommerce/src/Internal/PushNotifications/Services/NotificationPreferencesService.php
- plugins/woocommerce/src/Internal/PushNotifications/Traits/ConvertsExceptionsToWpError.php
- plugins/woocommerce/tests/php/src/Internal/PushNotifications/Controllers/NotificationPreferencesRestControllerTest.php

### #64348 Wire verify and confirmation emails for BIS alpha
https://github.com/woocommerce/woocommerce/pull/64348

Score: 4
Author: opr
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: rsm; keyword: stock notification
Touched areas:
- plugins/woocommerce/changelog/rsm-438-wire-bis-emails
- plugins/woocommerce/phpstan-baseline.neon
- plugins/woocommerce/src/Internal/StockNotifications/Admin/NotificationEditPage.php
- plugins/woocommerce/src/Internal/StockNotifications/Admin/NotificationsPage.php
- plugins/woocommerce/src/Internal/StockNotifications/Emails/CustomerStockNotificationEmail.php
- plugins/woocommerce/src/Internal/StockNotifications/Emails/CustomerStockNotificationVerifiedEmail.php
- plugins/woocommerce/src/Internal/StockNotifications/Emails/CustomerStockNotificationVerifyEmail.php
- plugins/woocommerce/src/Internal/StockNotifications/Emails/EmailActionController.php

### #64289 Add experimental Edge Cache Support for cart, checkout and mini-cart blocks
https://github.com/woocommerce/woocommerce/pull/64289

Score: 4
Author: jbouganim
Source search: All recent Woo PR activity: updated:>=2026-09-08
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

### #64250 [DataViews - All Products]: add @wordpress/theme package
https://github.com/woocommerce/woocommerce/pull/64250

Score: 4
Author: gigitux
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: keyword: dataviews; keyword: experiment
Touched areas:
- packages/js/experimental-products-app/changelog/add-wordpress-theme
- packages/js/experimental-products-app/package.json
- packages/js/experimental-products-app/src/app.tsx
- plugins/woocommerce/changelog/add-wordpress-theme
- plugins/woocommerce/client/admin/webpack.config.js
- pnpm-lock.yaml

### #65859 Add unique CSS classes to the order_data_column DIVs in the order edit screen
https://github.com/woocommerce/woocommerce/pull/65859

Score: 3
Author: webdados
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit
Touched areas:
- plugins/woocommerce/changelog/patch-1
- plugins/woocommerce/includes/admin/meta-boxes/class-wc-meta-box-order-data.php

### #65487 Fix tooltip accessibility: keyboard navigation, ARIA roles, and WCAG 1.4.13 compliance
https://github.com/woocommerce/woocommerce/pull/65487

Score: 3
Author: anuj-rathore24
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: path: plugins/woocommerce/includes/admin; keyword: navigation
Touched areas:
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-product.js
- plugins/woocommerce/client/legacy/js/admin/woocommerce_admin.js
- plugins/woocommerce/client/legacy/js/jquery-tiptip/jquery.tipTip.js
- plugins/woocommerce/includes/admin/meta-boxes/class-wc-meta-box-order-downloads.php
- plugins/woocommerce/includes/gateways/bacs/class-wc-gateway-bacs.php
- plugins/woocommerce/includes/wc-core-functions.php
- plugins/woocommerce/src/Internal/Admin/Orders/Edit.php

### #63396 Fix: shipping row style when Cost of Goods Sold is enabled on the order edit screen
https://github.com/woocommerce/woocommerce/pull/63396

Score: 3
Author: abdalsalaam
Source search: All recent Woo PR activity: updated:>=2026-09-08
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit
Touched areas:
- plugins/woocommerce/changelog/63396-fix-issue-63394
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-fee.php
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-refund.php
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-shipping.php
- plugins/woocommerce/includes/class-wc-ajax.php
- plugins/woocommerce/phpstan-baseline.neon

## Surface ownership policy

### Products table
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #68498 Fix the Settings > Emails listing styles by loading the listing on demand
Intent: feature-flag
Action: draft-pr
Designer review path: Products > All Products
Matched by: keyword: dataviews
Auto-merge: held; the bot should leave a draft PR for review.
- Product-list DataViews work is worth pulling forward, but feature-flagged UI changes should pause as a draft for review.

### Products table
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #65114 Polish the variations DataViews table and unify the stock pill
Intent: feature-flag
Action: draft-pr
Designer review path: Products > All Products
Matched by: keyword: dataviews
Auto-merge: held; the bot should leave a draft PR for review.
- Product-list DataViews work is worth pulling forward, but feature-flagged UI changes should pause as a draft for review.

### Products table
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #64243 [DataViews - All Products] Clean up code
Intent: feature-flag
Action: draft-pr
Designer review path: Products > All Products
Matched by: keyword: dataviews
Auto-merge: held; the bot should leave a draft PR for review.
- Product-list DataViews work is worth pulling forward, but feature-flagged UI changes should pause as a draft for review.

### Products table
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #64184 [Experimental] Create @woocommerce/experimental-products-app package (#64182)
Intent: feature-flag
Action: draft-pr
Designer review path: Products > All Products
Matched by: path: packages/js/product-editor
Auto-merge: held; the bot should leave a draft PR for review.
- Product-list DataViews work is worth pulling forward, but feature-flagged UI changes should pause as a draft for review.

### Products table
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #64182 Create @woocommerce/experimental-products-app package
Intent: feature-flag
Action: draft-pr
Designer review path: Products > All Products
Matched by: path: packages/js/product-editor
Auto-merge: held; the bot should leave a draft PR for review.
- Product-list DataViews work is worth pulling forward, but feature-flagged UI changes should pause as a draft for review.

### Products table
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #64250 [DataViews - All Products]: add @wordpress/theme package
Intent: feature-flag
Action: draft-pr
Designer review path: Products > All Products
Matched by: keyword: dataviews
Auto-merge: held; the bot should leave a draft PR for review.
- Product-list DataViews work is worth pulling forward, but feature-flagged UI changes should pause as a draft for review.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #68498 Fix the Settings > Emails listing styles by loading the listing on demand
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/client/admin/client/settings; path: plugins/woocommerce/includes/admin/settings
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #65893 [Backport to release/10.9] Rename @woocommerce/settings-ui-sdk to @woocommerce/settings-ui
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/client/admin/client/settings; path: plugins/woocommerce/includes/admin/settings; keyword: settings-ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #65729 [Backport to release/10.9] Align settings UI layout and number inputs with design spec
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #65719 Rename @woocommerce/settings-ui-sdk to @woocommerce/settings-ui
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/client/admin/client/settings; path: plugins/woocommerce/includes/admin/settings; keyword: settings-ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #65695 Align settings UI layout and number inputs with design spec
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #68684 [tests] Stop the Settings UI E2E spec from corrupting wp-env's cache
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
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
Woo PR: #68408 Simplify Settings UI updates and preserve extension registrations
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
Woo PR: #64711 Add prev/next order navigation to Order detail page header
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce admin rail
Matched by: keyword: navigation
Auto-merge: held; the bot should leave a draft PR for review.
- Navigation changes touch the frame of the whole prototype, so feature-flagged UI shifts should pause for review.

### Woo admin navigation
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #65487 Fix tooltip accessibility: keyboard navigation, ARIA roles, and WCAG 1.4.13 compliance
Intent: bugfix
Action: self-merge
Designer review path: WooCommerce admin rail
Matched by: keyword: navigation
- Navigation changes touch the frame of the whole prototype, so feature-flagged UI shifts should pause for review.

## Patch adapters

### Products table: DataViews adapter
Status: planned
Matched Woo PR: #68498 Fix the Settings > Emails listing styles by loading the listing on demand
Local target: client/dataviews-tables/products-list
Designer review path: Products > All Products
Matched by: keyword: dataviews
- Translate the Woo product-list DataViews surface into a Future Woo products-list bundle.
- Keep the adapter separate from the existing orders-list DataViews bundle until the Products page has its own smoke test.

### Products table: DataViews adapter
Status: planned
Matched Woo PR: #65114 Polish the variations DataViews table and unify the stock pill
Local target: client/dataviews-tables/products-list
Designer review path: Products > All Products
Matched by: keyword: dataviews
- Translate the Woo product-list DataViews surface into a Future Woo products-list bundle.
- Keep the adapter separate from the existing orders-list DataViews bundle until the Products page has its own smoke test.

### Products table: DataViews adapter
Status: planned
Matched Woo PR: #64243 [DataViews - All Products] Clean up code
Local target: client/dataviews-tables/products-list
Designer review path: Products > All Products
Matched by: keyword: dataviews
- Translate the Woo product-list DataViews surface into a Future Woo products-list bundle.
- Keep the adapter separate from the existing orders-list DataViews bundle until the Products page has its own smoke test.

### Products table: DataViews adapter
Status: planned
Matched Woo PR: #64184 [Experimental] Create @woocommerce/experimental-products-app package (#64182)
Local target: client/dataviews-tables/products-list
Designer review path: Products > All Products
Matched by: path: packages/js/product-editor
- Translate the Woo product-list DataViews surface into a Future Woo products-list bundle.
- Keep the adapter separate from the existing orders-list DataViews bundle until the Products page has its own smoke test.

### Products table: DataViews adapter
Status: planned
Matched Woo PR: #64182 Create @woocommerce/experimental-products-app package
Local target: client/dataviews-tables/products-list
Designer review path: Products > All Products
Matched by: path: packages/js/product-editor
- Translate the Woo product-list DataViews surface into a Future Woo products-list bundle.
- Keep the adapter separate from the existing orders-list DataViews bundle until the Products page has its own smoke test.

### Products table: DataViews adapter
Status: planned
Matched Woo PR: #64250 [DataViews - All Products]: add @wordpress/theme package
Local target: client/dataviews-tables/products-list
Designer review path: Products > All Products
Matched by: keyword: dataviews
- Translate the Woo product-list DataViews surface into a Future Woo products-list bundle.
- Keep the adapter separate from the existing orders-list DataViews bundle until the Products page has its own smoke test.

## Designer review paths

- Products > All Products
- WooCommerce admin rail
- WooCommerce > Settings

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

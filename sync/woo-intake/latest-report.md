# Future Woo intake report

Generated: 2026-07-28
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-07-21`.
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

### #66980 [Backport to release/11.0] Fix hidden Save button on Settings UI fallback pages
https://github.com/woocommerce/woocommerce/pull/66980

Score: 11
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/fix-66908-settings-ui-fallback-body-class
- plugins/woocommerce/includes/admin/settings/class-wc-settings-page.php
- plugins/woocommerce/tests/php/src/Internal/Admin/Settings/SettingsUIFeatureFlagTest.php

### #66958 Fix hidden Save button on Settings UI fallback pages
https://github.com/woocommerce/woocommerce/pull/66958

Score: 11
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/fix-66908-settings-ui-fallback-body-class
- plugins/woocommerce/includes/admin/settings/class-wc-settings-page.php
- plugins/woocommerce/tests/php/src/Internal/Admin/Settings/SettingsUIFeatureFlagTest.php

### #66866 Fix drill-down settings pages losing navigation on legacy fallback
https://github.com/woocommerce/woocommerce/pull/66866

Score: 11
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/fix-66664-drill-down-fallback-navigation
- plugins/woocommerce/includes/admin/views/html-admin-settings.php
- plugins/woocommerce/tests/php/src/Admin/Settings/SettingsSectionRegistryTest.php

### #66924 Stop the legacy header flash on Settings UI drill-down pages
https://github.com/woocommerce/woocommerce/pull/66924

Score: 9
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: path: plugins/woocommerce/client/admin/client/settings; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: navigation
Touched areas:
- packages/js/settings-ui/changelog/fix-error-boundary-onerror
- packages/js/settings-ui/src/settings-ui-page.tsx
- plugins/woocommerce/changelog/wooplug-7181-settings-ui-header-flash
- plugins/woocommerce/client/admin/client/settings/settings-ui-registry.tsx
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/settings-ui.scss

### #66939 [Backport to release/11.0] Mark the settings UI as experimental in the docs
https://github.com/woocommerce/woocommerce/pull/66939

Score: 8
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment
Touched areas:
- docs/extensions/settings-and-config/extend-wc-settings-page.md
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/README.md
- packages/js/settings-ui/changelog/dev-mark-package-experimental

### #66938 Mark the settings UI as experimental in the docs
https://github.com/woocommerce/woocommerce/pull/66938

Score: 8
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment
Touched areas:
- docs/extensions/settings-and-config/extend-wc-settings-page.md
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/README.md
- packages/js/settings-ui/changelog/dev-mark-package-experimental

### #66916 Preserve the legacy header when Settings UI fails to render
https://github.com/woocommerce/woocommerce/pull/66916

Score: 8
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/wooplug-7165-ai-regression-reviewtrunk-drill-down-css-hides-the-legacy
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/settings-ui.scss

### #66907 [Backport to release/11.0] Preserve navigation during Settings UI fallbacks
https://github.com/woocommerce/woocommerce/pull/66907

Score: 8
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/66664-fix-settings-ui-fallback-navigation
- plugins/woocommerce/includes/admin/views/html-admin-settings.php
- plugins/woocommerce/src/Admin/Settings/AGENTS.md
- plugins/woocommerce/tests/php/src/Admin/Settings/SettingsSectionRegistryTest.php

### #66668 Preserve navigation during Settings UI fallbacks
https://github.com/woocommerce/woocommerce/pull/66668

Score: 8
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/66664-fix-settings-ui-fallback-navigation
- plugins/woocommerce/includes/admin/settings/class-wc-settings-page.php
- plugins/woocommerce/includes/admin/views/html-admin-settings.php
- plugins/woocommerce/src/Admin/Settings/AGENTS.md
- plugins/woocommerce/tests/php/src/Admin/Settings/SettingsSectionRegistryTest.php

### #66854 Fix duplicate headers on Settings UI drill-down pages
https://github.com/woocommerce/woocommerce/pull/66854

Score: 7
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/wooprd-3585-settings-ui-drill-down-header
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/settings-ui.scss
- plugins/woocommerce/includes/admin/settings/class-wc-settings-page.php
- plugins/woocommerce/tests/php/src/Internal/Admin/Settings/SettingsUIFeatureFlagTest.php

### #66867 Add a visible focus indicator to the Settings UI shell tabs
https://github.com/woocommerce/woocommerce/pull/66867

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag
Touched areas:
- plugins/woocommerce/changelog/fix-settings-ui-shell-tab-focus-ring
- plugins/woocommerce/client/admin/client/wp-admin-scripts/settings-embed/settings-ui.scss

### #66689 Fix shipping recommendation dismissal accessibility and fallbacks
https://github.com/woocommerce/woocommerce/pull/66689

Score: 6
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: path: plugins/woocommerce/client/admin/client/shipping; path: plugins/woocommerce/includes/admin; keyword: navigation; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/wooplug-7093-shipping-recommendations-dismiss
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations.tsx
- plugins/woocommerce/client/admin/client/shipping/test/shipping-recommendations.test.tsx
- plugins/woocommerce/includes/admin/views/html-admin-settings.php
- plugins/woocommerce/tests/php/includes/admin/views/class-wc-admin-settings-view-test.php

### #66849 Fix shipping line names changing on order save
https://github.com/woocommerce/woocommerce/pull/66849

Score: 5
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/fix-66847-preserve-shipping-line-name
- plugins/woocommerce/includes/admin/wc-admin-functions.php
- plugins/woocommerce/tests/php/includes/admin/class-wc-admin-functions-test.php

### #66039 Add search and pagination to order tax modal
https://github.com/woocommerce/woocommerce/pull/66039

Score: 5
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit; author: j111q
Touched areas:
- plugins/woocommerce/changelog/add-tax-rate-modal-search-pagination
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/includes/admin/class-wc-admin-assets.php
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-items.php
- plugins/woocommerce/includes/class-wc-ajax.php
- plugins/woocommerce/tests/php/includes/class-wc-ajax-test.php

### #66955 [Backport to release/11.0] Fix boolean and visibility canonicalization in Settings UI schemas
https://github.com/woocommerce/woocommerce/pull/66955

Score: 4
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: keyword: settings-ui; keyword: settings ui
Touched areas:
- plugins/woocommerce/changelog/fix-66934-settings-ui-boolean-canonicalization
- plugins/woocommerce/src/Internal/Admin/Settings/RegisteredSettingsSectionAdapter.php
- plugins/woocommerce/src/Internal/Admin/Settings/SettingsUIRequestContext.php
- plugins/woocommerce/src/Internal/Admin/Settings/SettingsUISchema.php
- plugins/woocommerce/tests/php/src/Internal/Admin/Settings/SettingsUISchemaTest.php

### #66936 Fix boolean and visibility canonicalization in Settings UI schemas
https://github.com/woocommerce/woocommerce/pull/66936

Score: 4
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: keyword: settings-ui; keyword: settings ui
Touched areas:
- plugins/woocommerce/changelog/fix-66934-settings-ui-boolean-canonicalization
- plugins/woocommerce/src/Internal/Admin/Settings/RegisteredSettingsSectionAdapter.php
- plugins/woocommerce/src/Internal/Admin/Settings/SettingsUIRequestContext.php
- plugins/woocommerce/src/Internal/Admin/Settings/SettingsUISchema.php
- plugins/woocommerce/tests/php/src/Internal/Admin/Settings/SettingsUISchemaTest.php

### #66910 Revert "Make the dual API usable for plugins without the feature flag enabled"
https://github.com/woocommerce/woocommerce/pull/66910

Score: 4
Author: konamiman
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: keyword: feature flag; keyword: experiment
Touched areas:
- docs/apis/dual-api/README.md
- docs/apis/dual-api/caching-and-settings.md
- docs/apis/dual-api/creating-a-dual-api-in-a-plugin.md
- docs/apis/dual-api/reference/infrastructure-classes.md
- plugins/woocommerce/changelog/make-dual-api-usable-for-plugins-without-feature-enabled
- plugins/woocommerce/src/Api/Infrastructure/Main.php
- plugins/woocommerce/src/Internal/Api/Autogenerated/api_generation_date.txt
- plugins/woocommerce/src/Internal/Api/Autogenerated/api_source_hash.txt

### #66706 Make the dual API usable for plugins without the feature flag enabled
https://github.com/woocommerce/woocommerce/pull/66706

Score: 4
Author: konamiman
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: keyword: feature flag; keyword: experiment
Touched areas:
- docs/apis/dual-api/README.md
- docs/apis/dual-api/caching-and-settings.md
- docs/apis/dual-api/creating-a-dual-api-in-a-plugin.md
- docs/apis/dual-api/reference/infrastructure-classes.md
- plugins/woocommerce/changelog/make-dual-api-usable-for-plugins-without-feature-enabled
- plugins/woocommerce/src/Api/Infrastructure/Main.php
- plugins/woocommerce/src/Internal/Api/Autogenerated/api_generation_date.txt
- plugins/woocommerce/src/Internal/Api/Autogenerated/api_source_hash.txt

### #64289 Add experimental Edge Cache Support for cart, checkout and mini-cart blocks
https://github.com/woocommerce/woocommerce/pull/64289

Score: 4
Author: jbouganim
Source search: All recent Woo PR activity: updated:>=2026-07-21
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

### #66811 Fix shipping method names on manual orders
https://github.com/woocommerce/woocommerce/pull/66811

Score: 3
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: path: plugins/woocommerce/includes/admin; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/fix-manual-order-shipping-method-name
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/client/legacy/js/admin/test/meta-boxes-order.test.js
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-shipping.php
- plugins/woocommerce/includes/admin/wc-admin-functions.php
- plugins/woocommerce/tests/php/includes/admin/class-wc-admin-functions-test.php

### #66343 Clarify shipping zone save action when adding a method
https://github.com/woocommerce/woocommerce/pull/66343

Score: 3
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-07-21
Why it matched: path: plugins/woocommerce/includes/admin; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/update-shipping-zone-method-save-action
- plugins/woocommerce/includes/admin/settings/views/html-admin-page-shipping-zone-methods.php
- plugins/woocommerce/tests/e2e/tests/blocks/cart/cart-checkout-block-shipping.block_theme.spec.ts
- plugins/woocommerce/tests/e2e/tests/shipping/shipping-zones.spec.ts

## Surface ownership policy

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66980 [Backport to release/11.0] Fix hidden Save button on Settings UI fallback pages
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66958 Fix hidden Save button on Settings UI fallback pages
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings; keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66924 Stop the legacy header flash on Settings UI drill-down pages
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/client/admin/client/settings; keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66939 [Backport to release/11.0] Mark the settings UI as experimental in the docs
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66938 Mark the settings UI as experimental in the docs
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66916 Preserve the legacy header when Settings UI fails to render
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66907 [Backport to release/11.0] Preserve navigation during Settings UI fallbacks
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66668 Preserve navigation during Settings UI fallbacks
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings; keyword: settings-ui; keyword: settings ui
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66854 Fix duplicate headers on Settings UI drill-down pages
Intent: bugfix
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings; keyword: settings-ui; keyword: settings ui
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66867 Add a visible focus indicator to the Settings UI shell tabs
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66955 [Backport to release/11.0] Fix boolean and visibility canonicalization in Settings UI schemas
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66936 Fix boolean and visibility canonicalization in Settings UI schemas
Intent: bugfix
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66343 Clarify shipping zone save action when adding a method
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Shipping providers
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #66689 Fix shipping recommendation dismissal accessibility and fallbacks
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

### Woo admin navigation
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #66866 Fix drill-down settings pages losing navigation on legacy fallback
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce admin rail
Matched by: keyword: navigation
Auto-merge: held; the bot should leave a draft PR for review.
- Navigation changes touch the frame of the whole prototype, so feature-flagged UI shifts should pause for review.

### Woo admin navigation
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #66907 [Backport to release/11.0] Preserve navigation during Settings UI fallbacks
Intent: default
Action: draft-pr
Designer review path: WooCommerce admin rail
Matched by: keyword: navigation
Auto-merge: held; the bot should leave a draft PR for review.
- Navigation changes touch the frame of the whole prototype, so feature-flagged UI shifts should pause for review.

### Woo admin navigation
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #66668 Preserve navigation during Settings UI fallbacks
Intent: default
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
- WooCommerce > Settings
- WooCommerce > Settings > Shipping

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

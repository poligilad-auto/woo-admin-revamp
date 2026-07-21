# Future Woo intake report

Generated: 2026-07-21
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-07-14`.
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

### #66781 Settings UI: use the WordPress-bundled DataForm stack
https://github.com/woocommerce/woocommerce/pull/66781

Score: 15
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/client/admin/client/settings; path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: dataviews; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment; keyword: navigation
Touched areas:
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/README.md
- packages/js/settings-ui/changelog/update-dataform-renderer
- packages/js/settings-ui/package.json
- packages/js/settings-ui/src/dataform-adapter.tsx
- packages/js/settings-ui/src/diagnostics.ts
- packages/js/settings-ui/src/hidden-inputs.tsx

### #66758 Settings UI: render everything through DataForm on dataviews 17
https://github.com/woocommerce/woocommerce/pull/66758

Score: 12
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: dataviews; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment
Touched areas:
- .syncpackrc
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/changelog/update-dataform-renderer
- packages/js/settings-ui/jest.config.js
- packages/js/settings-ui/jest.config.json
- packages/js/settings-ui/package.json
- packages/js/settings-ui/src/dataform-adapter.tsx

### #66714 Settings UI: converge the renderer and extension contract on DataForm
https://github.com/woocommerce/woocommerce/pull/66714

Score: 12
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: keyword: dataviews; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment; keyword: navigation
Touched areas:
- .syncpackrc
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/changelog/fix-value-representation
- packages/js/settings-ui/changelog/update-dataform-renderer
- packages/js/settings-ui/package.json
- packages/js/settings-ui/src/dataform-adapter.tsx
- packages/js/settings-ui/src/hidden-inputs.tsx

### #66693 Converge the Settings UI renderer on DataForm
https://github.com/woocommerce/woocommerce/pull/66693

Score: 12
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: keyword: dataviews; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: experiment; keyword: navigation
Touched areas:
- docs/extensions/settings-and-config/registering-settings-ui-components.md
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/README.md
- packages/js/settings-ui/package.json
- packages/js/settings-ui/src/dataform-adapter.tsx
- packages/js/settings-ui/src/dataform-controls.tsx
- packages/js/settings-ui/src/index.ts
- packages/js/settings-ui/src/registry.ts

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

### #66686 Settings UI: render fields through DataForm (spike)
https://github.com/woocommerce/woocommerce/pull/66686

Score: 10
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: keyword: dataviews; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: navigation
Touched areas:
- packages/js/settings-ui/changelog/update-dataform-field-rendering
- packages/js/settings-ui/package.json
- packages/js/settings-ui/src/dataform-adapter.tsx
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/dataform-adapter.test.tsx
- pnpm-lock.yaml

### #66662 [Backport to release/11.0] Settings UI: shell header follows the page registration
https://github.com/woocommerce/woocommerce/pull/66662

Score: 10
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: navigation
Touched areas:
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/changelog/update-shell-header-top-level-pages
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/header-fields.test.tsx
- packages/js/settings-ui/src/test/html-rendering.test.tsx
- packages/js/settings-ui/src/test/shell-header-visibility.test.tsx
- packages/js/settings-ui/src/types.ts
- plugins/woocommerce/changelog/update-settings-ui-shell-header-top-level

### #66437 Settings UI: shell header follows the page registration
https://github.com/woocommerce/woocommerce/pull/66437

Score: 10
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/src/Admin; path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: feature flag; keyword: navigation
Touched areas:
- docs/extensions/settings-and-config/settings-ui.md
- packages/js/settings-ui/changelog/update-shell-header-top-level-pages
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/header-fields.test.tsx
- packages/js/settings-ui/src/test/html-rendering.test.tsx
- packages/js/settings-ui/src/test/shell-header-visibility.test.tsx
- packages/js/settings-ui/src/types.ts
- plugins/woocommerce/changelog/update-settings-ui-shell-header-top-level

### #66668 Preserve navigation during Settings UI fallbacks
https://github.com/woocommerce/woocommerce/pull/66668

Score: 7
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/includes/admin; keyword: settings-ui; keyword: settings ui; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/66664-fix-settings-ui-fallback-navigation
- plugins/woocommerce/includes/admin/views/html-admin-settings.php
- plugins/woocommerce/tests/php/src/Admin/Settings/SettingsSectionRegistryTest.php

### #66689 Fix shipping recommendation dismissal accessibility and fallbacks
https://github.com/woocommerce/woocommerce/pull/66689

Score: 6
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/client/admin/client/shipping; path: plugins/woocommerce/includes/admin; keyword: navigation; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/wooplug-7093-shipping-recommendations-dismiss
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations.tsx
- plugins/woocommerce/client/admin/client/shipping/test/shipping-recommendations.test.tsx
- plugins/woocommerce/includes/admin/views/html-admin-settings.php
- plugins/woocommerce/tests/php/includes/admin/views/class-wc-admin-settings-view-test.php

### #66561 [Settings UI] Fix value matching for extension-supplied schemas
https://github.com/woocommerce/woocommerce/pull/66561

Score: 6
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: keyword: settings-ui; keyword: settings ui; keyword: feature flag
Touched areas:
- packages/js/settings-ui/changelog/fix-select-option-value-coercion
- packages/js/settings-ui/src/checkbox-values.ts
- packages/js/settings-ui/src/hidden-inputs.tsx
- packages/js/settings-ui/src/native-fields.tsx
- packages/js/settings-ui/src/settings-ui-page.tsx
- packages/js/settings-ui/src/test/header-fields.test.tsx
- packages/js/settings-ui/src/test/hidden-inputs.test.ts
- packages/js/settings-ui/src/test/html-rendering.test.tsx

### #62784 Exploration: Add React-based General Settings UI
https://github.com/woocommerce/woocommerce/pull/62784

Score: 6
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/client/admin/client/settings; path: plugins/woocommerce/includes/admin; keyword: settings ui; keyword: feature flag
Touched areas:
- plugins/woocommerce/client/admin/client/settings-general/hooks/use-general-settings.ts
- plugins/woocommerce/client/admin/client/settings-general/index.tsx
- plugins/woocommerce/client/admin/client/settings-general/settings-general-main.scss
- plugins/woocommerce/client/admin/client/settings-general/settings-general-main.tsx
- plugins/woocommerce/client/admin/client/settings-general/settings-general-slotfill.tsx
- plugins/woocommerce/client/admin/client/settings-general/test/settings-general-main.test.tsx
- plugins/woocommerce/client/admin/client/settings-general/utils.js
- plugins/woocommerce/client/admin/client/settings/settings-slots.js

### #66039 Add search and pagination to order tax modal
https://github.com/woocommerce/woocommerce/pull/66039

Score: 5
Author: j111q
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit; author: j111q
Touched areas:
- plugins/woocommerce/changelog/add-tax-rate-modal-search-pagination
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/includes/admin/class-wc-admin-assets.php
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-items.php
- plugins/woocommerce/includes/class-wc-ajax.php
- plugins/woocommerce/tests/php/includes/class-wc-ajax-test.php

### #66706 Make the dual API usable for plugins without the feature flag enabled
https://github.com/woocommerce/woocommerce/pull/66706

Score: 4
Author: konamiman
Source search: All recent Woo PR activity: updated:>=2026-07-14
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

### #66593 Document Settings UI native controls
https://github.com/woocommerce/woocommerce/pull/66593

Score: 4
Author: dmallory42
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: keyword: settings-ui; keyword: settings ui
Touched areas:
- docs/extensions/settings-and-config/settings-ui.md

### #66418 Fix false "unsaved changes"/"Leave site?" warning on the order edit screen
https://github.com/woocommerce/woocommerce/pull/66418

Score: 4
Author: towytowy
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: keyword: order edit; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/66418-fix-order-edit-unsaved-changes-warning
- plugins/woocommerce/changelog/fix-66308-order-edit-unsaved-changes-warning
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js

### #66110 Fix duplicate shipping marketplace link
https://github.com/woocommerce/woocommerce/pull/66110

Score: 4
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/client/admin/client/shipping; path: plugins/woocommerce/includes/admin; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/fix-duplicate-shipping-marketplace-link
- plugins/woocommerce/client/admin/client/hooks/test/use-endpoint-dismiss.test.ts
- plugins/woocommerce/client/admin/client/hooks/test/use-option-dismiss.test.ts
- plugins/woocommerce/client/admin/client/hooks/use-endpoint-dismiss.ts
- plugins/woocommerce/client/admin/client/hooks/use-option-dismiss.ts
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations-utils.tsx
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations.scss
- plugins/woocommerce/client/admin/client/shipping/shipping-recommendations.tsx

### #66811 Fix shipping method names on manual orders
https://github.com/woocommerce/woocommerce/pull/66811

Score: 3
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/includes/admin; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/fix-manual-order-shipping-method-name
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-shipping.php
- plugins/woocommerce/includes/admin/wc-admin-functions.php
- plugins/woocommerce/tests/php/includes/admin/class-wc-admin-functions-test.php

### #66676 [Backport to release/11.0] Fix order edit AJAX error and prevent `autosave.js` from loading on WC screens
https://github.com/woocommerce/woocommerce/pull/66676

Score: 3
Author: woocommercebot
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit
Touched areas:
- plugins/woocommerce/changelog/66411-fix-order-edit-sample-permalink-403
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/client/legacy/js/admin/woocommerce_admin.js
- plugins/woocommerce/includes/admin/class-wc-admin-assets.php
- plugins/woocommerce/includes/admin/meta-boxes/class-wc-meta-box-order-data.php
- plugins/woocommerce/readme.txt
- plugins/woocommerce/tests/e2e/tests/order/order-edit.spec.ts
- plugins/woocommerce/tests/php/includes/admin/class-wc-admin-assets-test.php

### #66579 Fix order edit AJAX error and prevent `autosave.js` from loading on WC screens
https://github.com/woocommerce/woocommerce/pull/66579

Score: 3
Author: jorgeatorres
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit
Touched areas:
- plugins/woocommerce/changelog/66411-fix-order-edit-sample-permalink-403
- plugins/woocommerce/client/legacy/css/admin.scss
- plugins/woocommerce/client/legacy/js/admin/woocommerce_admin.js
- plugins/woocommerce/includes/admin/class-wc-admin-assets.php
- plugins/woocommerce/includes/admin/meta-boxes/class-wc-meta-box-order-data.php
- plugins/woocommerce/tests/e2e/tests/order/order-edit.spec.ts
- plugins/woocommerce/tests/php/includes/admin/class-wc-admin-assets-test.php

### #66348 Add warnings for shadowed shipping zones
https://github.com/woocommerce/woocommerce/pull/66348

Score: 3
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/includes/admin; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/30340-shipping-zone-order-warning
- plugins/woocommerce/includes/admin/settings/class-wc-settings-shipping.php
- plugins/woocommerce/includes/admin/settings/views/html-admin-page-shipping-zones.php
- plugins/woocommerce/includes/class-wc-ajax.php
- plugins/woocommerce/includes/class-wc-shipping-zones.php
- plugins/woocommerce/tests/php/includes/class-wc-shipping-zones-test.php

### #66343 Fix shipping zone save button after adding method
https://github.com/woocommerce/woocommerce/pull/66343

Score: 3
Author: annchichi
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/includes/admin; author: annchichi
Touched areas:
- plugins/woocommerce/changelog/update-shipping-zone-method-save-action
- plugins/woocommerce/includes/admin/settings/views/html-admin-page-shipping-zone-methods.php
- plugins/woocommerce/tests/e2e/tests/blocks/cart/cart-checkout-block-shipping.block_theme.spec.ts
- plugins/woocommerce/tests/e2e/tests/shipping/shipping-zones.spec.ts

### #62953 WooCommerce settings feature flag
https://github.com/woocommerce/woocommerce/pull/62953

Score: 3
Author: elazzabi
Source search: All recent Woo PR activity: updated:>=2026-07-14
Why it matched: path: plugins/woocommerce/client/admin/client/settings; keyword: feature flag
Touched areas:
- plugins/woocommerce-react-settings-custom-field/build-custom-field.sh
- plugins/woocommerce-react-settings-custom-field/custom-field.css
- plugins/woocommerce-react-settings-custom-field/custom-field.js
- plugins/woocommerce-react-settings-custom-field/custom-field.tsx
- plugins/woocommerce-react-settings-custom-field/woocommerce-react-settings-custom-field.php
- plugins/woocommerce-react-settings-test/woocommerce-react-settings-test.php
- plugins/woocommerce/client/admin/client/settings-general/config.ts
- plugins/woocommerce/client/admin/client/settings/field-transformers.js

## Surface ownership policy

### Products table
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #66758 Settings UI: render everything through DataForm on dataviews 17
Intent: feature-flag
Action: draft-pr
Designer review path: Products > All Products
Matched by: keyword: dataviews
Auto-merge: held; the bot should leave a draft PR for review.
- Product-list DataViews work is worth pulling forward, but feature-flagged UI changes should pause as a draft for review.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66781 Settings UI: use the WordPress-bundled DataForm stack
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/client/admin/client/settings; path: plugins/woocommerce/includes/admin/settings; keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66758 Settings UI: render everything through DataForm on dataviews 17
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings; keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66714 Settings UI: converge the renderer and extension contract on DataForm
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66693 Converge the Settings UI renderer on DataForm
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66686 Settings UI: render fields through DataForm (spike)
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66662 [Backport to release/11.0] Settings UI: shell header follows the page registration
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66437 Settings UI: shell header follows the page registration
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66668 Preserve navigation during Settings UI fallbacks
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66561 [Settings UI] Fix value matching for extension-supplied schemas
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: keyword: settings-ui; keyword: settings ui
Auto-merge: held; the bot should leave a draft PR for review.
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #62784 Exploration: Add React-based General Settings UI
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/client/admin/client/settings; path: plugins/woocommerce/includes/admin/settings; keyword: settings ui
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

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66348 Add warnings for shadowed shipping zones
Intent: default
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #66343 Fix shipping zone save button after adding method
Intent: bugfix
Action: self-merge
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/includes/admin/settings
- Settings currently behaves like a mirror surface, so low-risk Woo improvements can flow in automatically when checks pass.

### Settings screens
Mode: mirror-owned
Owner: Woo core
Woo PR: #62953 WooCommerce settings feature flag
Intent: feature-flag
Action: draft-pr
Designer review path: WooCommerce > Settings
Matched by: path: plugins/woocommerce/client/admin/client/settings
Auto-merge: held; the bot should leave a draft PR for review.
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

### Shipping providers
Mode: hybrid
Owner: Future Woo plus Woo core
Woo PR: #66110 Fix duplicate shipping marketplace link
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
Woo PR: #66668 Preserve navigation during Settings UI fallbacks
Intent: default
Action: draft-pr
Designer review path: WooCommerce admin rail
Matched by: keyword: navigation
Auto-merge: held; the bot should leave a draft PR for review.
- Navigation changes touch the frame of the whole prototype, so feature-flagged UI shifts should pause for review.

## Patch adapters

### Products table: DataViews adapter
Status: planned
Matched Woo PR: #66758 Settings UI: render everything through DataForm on dataviews 17
Local target: client/dataviews-tables/products-list
Designer review path: Products > All Products
Matched by: keyword: dataviews
- Translate the Woo product-list DataViews surface into a Future Woo products-list bundle.
- Keep the adapter separate from the existing orders-list DataViews bundle until the Products page has its own smoke test.

## Designer review paths

- Products > All Products
- WooCommerce admin rail
- WooCommerce > Settings
- WooCommerce > Settings > Shipping

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

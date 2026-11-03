# Future Woo intake report

Generated: 2026-11-03
Source: woocommerce/woocommerce
Auto-merge gate: hold

## What the bot checked

- All recent Woo PR activity: all PRs matching `updated:>=2026-10-27`.
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

### #70550 Allow decimal quantity for order items in the admin order editor
https://github.com/woocommerce/woocommerce/pull/70550

Score: 5
Author: anuj-rathore24
Source search: All recent Woo PR activity: updated:>=2026-10-27
Why it matched: path: plugins/woocommerce/includes/admin; keyword: order edit; keyword: navigation
Touched areas:
- plugins/woocommerce/changelog/fix-order-item-qty-step-validation
- plugins/woocommerce/client/legacy/js/admin/meta-boxes-order.js
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-item.php
- plugins/woocommerce/includes/admin/meta-boxes/views/html-order-items.php
- plugins/woocommerce/includes/class-wc-ajax.php
- plugins/woocommerce/src/Internal/Admin/Orders/ItemQuantityLimits.php
- plugins/woocommerce/tests/e2e/tests/order/order-item-quantity-validation.spec.ts
- plugins/woocommerce/tests/php/includes/class-wc-ajax-test.php

### #70328 Agent readiness: product and store checks behind a feature flag
https://github.com/woocommerce/woocommerce/pull/70328

Score: 4
Author: annamag
Source search: All recent Woo PR activity: updated:>=2026-10-27
Why it matched: keyword: feature flag; keyword: experiment
Touched areas:
- plugins/woocommerce/changelog/add-agent-readiness-status
- plugins/woocommerce/includes/class-woocommerce.php
- plugins/woocommerce/src/Internal/AgentReadiness/AgentReadiness.php
- plugins/woocommerce/src/Internal/AgentReadiness/Checks/AbstractReadinessCheck.php
- plugins/woocommerce/src/Internal/AgentReadiness/Checks/DuplicateGtinCheck.php
- plugins/woocommerce/src/Internal/AgentReadiness/Checks/ImageTooSmallCheck.php
- plugins/woocommerce/src/Internal/AgentReadiness/Checks/MissingBrandCheck.php
- plugins/woocommerce/src/Internal/AgentReadiness/Checks/MissingGtinCheck.php

## Surface ownership policy

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

## How to read this

- If the gate says `merge`, the bot is allowed to merge this PR after it creates it.
- If the gate says `hold`, the bot leaves a draft PR and this report is the handoff.
- A candidate here is not a promise that the patch applied. It is a designer-relevant Woo change the bot noticed and tried to keep visible.

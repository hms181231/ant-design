---
group:
  title: Migration
order: 1
title: Less variables to Component Token
---

This document contains the correspondence between all the less variables related to components in version 4.x and the Component Token in version 5.x. If you are upgrading from version 4.x to version 5.x, you can quickly find the corresponding Component Token through this comparison table.

<Alert message="Note: There are still some less variables that do not have a corresponding Component Token, and these variables have been deprecated in version 5.x."></Alert>

## How to use Component Token

We could configure global token and component token for each component through the `theme` property of ConfigProvider.

```tsx
import React from 'react';
import { Checkbox, ConfigProvider, Radio } from 'antd';

const App: React.FC = () => (
  <ConfigProvider
    theme={{
      components: {
        Radio: {
          colorPrimary: '#00b96b',
        },
        Checkbox: {
          colorPrimary: '#ff4d4f',
        },
      },
    }}
  >
    <Radio>Radio</Radio>
    <Checkbox>Checkbox</Checkbox>
  </ConfigProvider>
);

export default App;
```

<!-- ## 全局变量 -->

## Component Token

<!-- ### Alert -->

### Anchor

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@anchor-bg` | '-' | Can be modified directly by `className` or `style` |
| `@anchor-border-color` | `colorSplit` | GlobalToken |
| `@anchor-link-top` | `linkPaddingBlock` | - |
| `@anchor-link-left` | `linkPaddingInlineStart` | - |
| `@anchor-link-padding` | - | `${linkPaddingBlock}px ${linkPaddingInlineStart}px` |

### Avatar

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@avatar-size-base` | `containerSize` | - |
| `@avatar-size-lg` | `containerSizeLG` | - |
| `@avatar-size-sm` | `containerSizeSM` | - |
| `@avatar-font-size-base` | `textFontSize` | - |
| `@avatar-font-size-lg` | `textFontSizeLG` | - |
| `@avatar-font-size-sm` | `textFontSizeSM` | - |
| `@avatar-bg` | - | Can be directly overridden by `className` or `style` |
| `@avatar-color` | `colorTextLightSolid` | Global Token |
| `@avatar-border-radius` | `borderRadius` | Global Token |
| `@avatar-group-overlapping` | - | Deprecated for style change |
| `@avatar-group-space` | `groupSpace` | - |
| `@avatar-group-border-color` | `colorBorderBg` | Global Token |

<!-- ### Badge -->

### BreadCrumb

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@breadcrumb-base-color` | `itemColor` | - |
| `@breadcrumb-last-item-color` | `lastItemColor` | - |
| `@breadcrumb-font-size` | `fontSize` | GlobalToken |
| `@breadcrumb-icon-font-size` | `iconFontSize` | - |
| `@breadcrumb-link-color` | `linkColor` | - |
| `@breadcrumb-link-color-hover` | `linkHoverColor` | - |
| `@breadcrumb-separator-color` | `separatorColor` | - |
| `@breadcrumb-separator-margin` | `separatorMargin` | - |

### Button

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@btn-font-weight` | `fontWeight` | - |
| `@btn-border-radius-base` | `borderRadius` | Global Token |
| `@btn-border-radius-sm` | `borderRadisuSM` | Global Token |
| `@btn-border-width` | `lineWidth` | Global Token |
| `@btn-border-style` | `lineStyle` | Global Token |
| `@btn-shadow` | `defaultShadow` | - |
| `@btn-primary-shadow` | `primaryShadow` | - |
| `@btn-text-shadow` | - | Deprecated for no `text-shadow` any more |
| `@btn-primary-color` | `primaryColor` | - |
| `@btn-primary-bg` | `colorPrimary` | Global Token |
| `@btn-default-color` | `colorText` | Global Token |
| `@btn-default-bg` | `colorBgContainer` | Global Token |
| `@btn-default-border` | `colorBorder` | Global Token |
| `@btn-danger-color` | `dangerColor` | - |
| `@btn-danger-bg` | `colorError` | Global Token |
| `@btn-danger-border` | `colorError` | Global Token |
| `@btn-disable-color` | `colorTextDisabled` | Global Token |
| `@btn-disable-bg` | `colorBgContainerDisabled` | Global Token |
| `@btn-disable-border` | `borderColorDisabled` | - |
| `@btn-default-ghost-color` | `defaultGhostColor` | - |
| `@btn-default-ghost-bg` | `ghostBg` | - |
| `@btn-default-ghost-border` | `defaultGhostBorderColor` | - |
| `@btn-font-size-lg` | `fontSizeLG` | Global Token |
| `@btn-font-size-sm` | `fontSizeSM` | Global Token |
| `@btn-padding-horizontal-base` | `paddingInline` | - |
| `@btn-padding-horizontal-lg` | `paddingInlineLG` | - |
| `@btn-padding-horizontal-sm` | `paddingInlineSM` | - |
| `@btn-height-base` | `controlHeight` | Global Token |
| `@btn-height-lg` | `controlHeightLG` | Global Token |
| `@btn-height-sm` | `controlHeightSM` | Global Token |
| `@btn-line-height` | `lineHeight` | Global Token |
| `@btn-circle-size` | `controlHeight` | Global Token |
| `@btn-circle-size-lg` | `controlHeightLG` | Global Token |
| `@btn-circle-size-sm` | `controlHeightSM` | Global Token |
| `@btn-square-size` | `controlHeight` | Global Token |
| `@btn-square-size-lg` | `controlHeightLG` | Global Token |
| `@btn-square-size-sm` | `controlHeightSM` | Global Token |
| `@btn-square-only-icon-size` | `onlyIconSize` | - |
| `@btn-square-only-icon-size-sm` | `onlyIconSizeSM` | - |
| `@btn-square-only-icon-size-lg` | `onlyIconSizeLG` | - |
| `@btn-group-border` | `groupBorderColor` | - |
| `@btn-link-hover-bg` | `linkHoverBg` | - |
| `@btn-text-hover-bg` | `textHoverBg` | - |

### Calendar

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@calendar-bg` | - | Deprecated for style change |
| `@calendar-input-bg` | - | Deprecated for style change |
| `@calendar-border-color` | - | Deprecated for style change |
| `@calendar-item-active-bg` | `itemActiveBg` | - |
| `@calendar-column-active-bg` | - | Deprecated for style change |
| `@calendar-full-bg` | `fullBg` | - |
| `@calendar-full-panel-bg` | `fullPanelBg` | - |

### Card

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@card-head-color` | `colorTextHeading` | Global Token |
| `@card-head-background` | `headerBg` | - |
| `@card-head-font-size` | `headerFontSize` | - |
| `@card-head-font-size-sm` | `headerFontSizeSM` | - |
| `@card-head-padding` | - | Deprecated |
| `@card-head-padding-sm` | - | Deprecated |
| `@card-head-height` | `headerHeight` | - |
| `@card-head-height-sm` | `headerHeightSM` | - |
| `@card-inner-head-padding` | - | Deprecated |
| `@card-padding-base` | `cardPaddingBase` | - |
| `@card-padding-base-sm` | `cardPaddingBaseSm` | - |
| `@card-actions-background` | `actionsBackground` | - |
| `@card-actions-li-margin` | `actionsLiMargin` | - |
| `@card-skeleton-bg` | - | Deprecated in favor of internal Skeleton |
| `@card-background` | `colorBgContainer` | Global Token |
| `@card-shadow` | - | Could be modified by `className` or `style` directly |
| `@card-radius` | `borderRadiusLG` | Global Token |
| `@card-head-tabs-margin-bottom` | `tabsMarginBottom` | - |
| `@card-head-extra-color` | `extraColor` | - |

### Carousel

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@carousel-dot-width` | `dotWidth` | - |
| `@carousel-dot-height` | `dotHeight` | - |
| `@carousel-dot-active-width` | `dotActiveWidth` | - |

<!-- ### Cascader -->

<!-- ### Checkbox -->

### Checkbox

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@checkbox-size` | `controlInteractiveSize` | GlobalToken |
| `@checkbox-color` | `colorPrimary` | - |
| `@checkbox-check-color` | `colorWhite` | - |
| `@checkbox-check-bg` | - | `colorPrimary` |
| `@checkbox-border-width` | `lineWidth` | - |
| `@checkbox-border-radius` | `borderRadiusSM` | - |
| `@checkbox-group-item-margin-right` | - | Deprecated for style change |

<!-- ### Collapse -->

### Descriptions

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@descriptions-bg` | `labelBg` | - |
| `@descriptions-title-margin-bottom` | `titleMarginBottom` | - |
| `@descriptions-default-padding` | `padding`、`paddingLG` | GlobalToken, used as `${token.padding}px ${token.paddingLG}px` |
| `@descriptions-middle-padding` | `paddingSM`、`paddingLG` | GlobalToken, used as `${token.paddingSM}px ${token.paddingLG}px` |
| `@descriptions-small-padding` | `paddingXS`、`padding` | GlobalToken, used as `${token.paddingXS}px ${token.padding}px` |
| `@descriptions-item-padding-bottom` | `itemPaddingBottom` | - |
| `@descriptions-item-trailing-colon` | - | Deprecated for style change |
| `@descriptions-item-label-colon-margin-right` | `colonMarginRight` | - |
| `@descriptions-item-label-colon-margin-left` | `colonMarginLeft` | - |
| `@descriptions-extra-color` | `extraColor` | - |

### Divider

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| --- | --- | --- |
| `@divider-text-padding` | `textPaddingInline` | - |
| `@divider-orientation-margin` | `orientationMargin` | - |
| `@divider-color` | `colorSplit` | Global Token |
| `@divider-vertical-gutter` | `verticalMarginInline` | - |

### Drawer

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@drawer-bg` | `colorBgElevated` | GlobalToken |
| `@drawer-header-padding` | `padding`、`paddingLG` | GlobalToken, used as `${padding}px ${paddingLG}px` |
| `@drawer-title-font-size` | `fontSizeLG` | GlobalToken |
| `@drawer-title-line-height` | `lineHeightLG` | GlobalToken |
| `@drawer-body-padding` | `paddingLG` | GlobalToken |
| `@drawer-footer-padding-vertical` | `footerPaddingBlock` | `footerPaddingBlock`  is a number without units, `@drawer-footer-padding-vertical` with units |
| `@drawer-footer-padding-horizontal` | `footerPaddingInline` | `footerPaddingInline`  is a number without units, `@drawer-footer-padding-horizontal` with units |

### Dropdown

| Less variables                       | Component Token       | Note        |
| ------------------------------------ | --------------------- | ----------- |
| `@dropdown-selected-color`           | `colorPrimary`        | -           |
| `@dropdown-menu-submenu-disabled-bg` | `colorBgElevated`     | GlobalToken |
| `@dropdown-selected-bg`              | `controlItemBgActive` | GlobalToken |

### Empty

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@empty-font-size` | `fontSize` | GlobalToken |

<!-- ### Form -->

### Image

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@image-size-base` | - | Deprecated for not used |
| `@image-font-size-base` | - | Deprecated for not used |
| `@image-bg` | `colorFillTertiary` | GlobalToken |
| `@image-color` | `colorTextLightSolid` | GlobalToken |
| `@image-preview-operation-size` | `previewOperationSize` | - |
| `@image-preview-operation-color` | `previewOperationColor` | - |
| `@image-preview-operation-disabled-color` | `previewOperationColorDisabled` | - |

<!-- ### Input -->

### Layout

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@layout-body-background` | `bodyBg` | - |
| `@layout-header-background` | `headerBg` | - |
| `@layout-header-height` | `headerHeight` | - |
| `@layout-header-padding` | `headerPadding` | - |
| `@layout-header-color` | `headerColor` | - |
| `@layout-footer-padding` | `footerPadding` | - |
| `@layout-footer-background` | `footerBg` | - |
| `@layout-sider-background` | `siderBg` | - |
| `@layout-trigger-height` | `triggerHeight` | - |
| `@layout-trigger-background` | `triggerBg` | - |
| `@layout-trigger-color` | `triggerColor` | - |
| `@layout-zero-trigger-width` | `zeroTriggerWidth` | - |
| `@layout-zero-trigger-height` | `zeroTriggerHeight` | - |
| `@layout-sider-background-light` | `lightSiderBg` | - |
| `@layout-trigger-background-light` | `lightTriggerBg` | - |
| `@layout-trigger-color-light` | `lightTriggerColor` | - |

### List

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@list-header-background` | `headerBg` | - |
| `@list-footer-background` | `footerBg` | - |
| `@list-empty-text-padding` | `emptyTextPadding` | - |
| `@list-item-padding` | `itemPadding` | - |
| `@list-item-padding-sm` | `itemPaddingSM` | - |
| `@list-item-padding-lg` | `itemPaddingLG` | - |
| `@list-item-meta-margin-bottom` | `metaMarginBottom` | - |
| `@list-item-meta-avatar-margin-right` | `avatarMarginRight` | - |
| `@list-item-meta-title-margin-bottom` | `titleMarginBottom` | - |
| `@list-customize-card-bg` | - | Deprecated for style change |
| `@list-item-meta-description-font-size` | `descriptionFontSize` | - |

### Mentions

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@mentions-dropdown-bg` | `colorBgElevated` | GlobalToken |
| `@mentions-dropdown-menu-item-hover-bg` | - | Deprecated |

### Menu

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@menu-inline-toplevel-item-height` | `itemHeight` | Same as `@menu-item-height` |
| `@menu-item-height` | `itemHeight` | - |
| `@menu-item-group-height` | `groupTitleLineHeight` | - |
| `@menu-collapsed-width` | `collapsedWidth` | - |
| `@menu-bg` | `itemBg` | - |
| `@menu-popup-bg` | `popupBg` | - |
| `@menu-item-color` | `itemColor` | - |
| `@menu-inline-submenu-bg` | `subMenuItemBg` | - |
| `@menu-highlight-color` | `itemSelectedColor` | - |
| `@menu-highlight-danger-color` | `dangerItemSelectedColor` | - |
| `@menu-item-active-bg` | `itemActiveBg` | - |
| `@menu-item-active-danger-bg` | `dangerItemActiveBg` | - |
| `@menu-item-active-border-width` | `activeBarBorderWidth` | - |
| `@menu-item-group-title-color` | `groupTitleColor` | - |
| `@menu-item-vertical-margin` | `itemMarginBlock` | - |
| `@menu-item-font-size` | `fontSize` | Global Token |
| `@menu-item-boundary-margin` | - | Deprecated in favor of new style, use `itemMarginBlock` instead |
| `@menu-item-padding-horizontal` | `itemPaddingInline` | - |
| `@menu-item-padding` | - | Depreacated, use `itemPaddingInline` and `itemHeight` instead |
| `@menu-horizontal-line-height` | `horizontalLineHeight` | - |
| `@menu-icon-margin-right` | `iconMarginInlineEnd` | - |
| `@menu-icon-size` | `iconSize` | - |
| `@menu-icon-size-lg` | `horizontalLineHeight` | - |
| `@menu-dark-color` | `darkItemColor` | - |
| `@menu-dark-danger-color` | `darkDangerItemColor` | - |
| `@menu-dark-bg` | `darkItemBg` | - |
| `@menu-dark-arrow-color` | - | Deprecated, and same as text color |
| `@menu-dark-inline-submenu-bg` | `darkSubMenuItemBg` | - |
| `@menu-dark-highlight-color` | `darkItemSelectedColor` | - |
| `@menu-dark-item-active-bg` | `darkItemSelectedBg` | - |
| `@menu-dark-item-active-danger-bg` | `darkDangerItemSelectedBg` | - |
| `@menu-dark-selected-item-icon-color` | - | Deprecated, same as `darkItemSelectedColor` |
| `@menu-dark-selected-item-text-color` | - | Deprecated, same as `darkItemSelectedColor` |
| `@menu-dark-item-hover-bg` | `darkItemHoverBg` | - |

### Message

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@zindex-message` | `zIndexPopup` | - |
| `@message-notice-content-padding` | `contentPadding` | - |
| `@message-notice-content-bg` | `contentBg` | - |

### Modal

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@modal-header-padding-vertical` | - | Deprecated for style change |
| `@modal-header-padding-horizontal` | - | Deprecated for style change |
| `@modal-body-padding` | - | Deprecated for style change |
| `@modal-header-bg` | `headerBg` | - |
| `@modal-header-padding` | - | Deprecated for style change |
| `@modal-header-border-width` | - | Deprecated for style change |
| `@modal-header-border-style` | - | Deprecated for style change |
| `@modal-header-title-line-height` | `titleLineHeight` | - |
| `@modal-header-title-font-size` | `titleFontSize` | - |
| `@modal-header-border-color-split` | - | Deprecated for style change |
| `@modal-header-close-size` | - | Deprecated for style change |
| `@modal-content-bg` | `contentBg` | - |
| `@modal-heading-color` | `titleColor` | - |
| `@modal-close-color` | `colorIcon` | GlobalToken |
| `@modal-footer-bg` | `footerBg` | - |
| `@modal-footer-border-color-split` | - | Deprecated for style change |
| `@modal-footer-border-style` | - | Deprecated for style change |
| `@modal-footer-padding-vertical` | - | Deprecated for style change |
| `@modal-footer-padding-horizontal` | - | Deprecated for style change |
| `@modal-footer-border-width` | - | Deprecated for style change |
| `@modal-mask-bg` | `colorBgMask` | GlobalToken |
| `@modal-confirm-body-padding` | - | Deprecated for style change |
| `@modal-confirm-title-font-size` | `titleFontSize` | - |
| `@modal-border-radius` | `borderRadiusLG` | GlobalToken |

<!-- ### Notification -->

### Pagination

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@pagination-item-bg` | `itemBg` | - |
| `@pagination-item-size` | `itemSize` | - |
| `@pagination-item-size-sm` | `itemSizeSM` | - |
| `@pagination-font-family` | `fontFamily` | GlobalToken |
| `@pagination-font-weight-active` | `fontWeightStrong` | GlobalToken |
| `@pagination-item-bg-active` | `itemActiveBg` | - |
| `@pagination-item-link-bg` | `itemLinkBg` | - |
| `@pagination-item-disabled-color-active` | `itemDisabledColorActive` | - |
| `@pagination-item-disabled-bg-active` | `itemDisabledBgActive` | - |
| `@pagination-item-input-bg` | `itemInputBg` | - |
| `@pagination-mini-options-size-changer-top` | `miniOptionsSizeChangerTop` | - |

### Popover>

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@popover-bg` | `colorBgContainer` | - |
| `@popover-color` | `colorText` | GlobalToken |
| `@popover-min-width` | `minWidth` | - |
| `@popover-min-height` | - | Deprecated  for style change |
| `@popover-arrow-width` | `sizePopupArrow` | GlobalToken |
| `@popover-arrow-color` | - | Deprecated  for style change |
| `@popover-arrow-outer-color` | - | Deprecated  for style change |
| `@popover-distance` | `marginXXS` | Global Token |
| `@popover-padding-horizontal` | - | Deprecated for style change |

### Progress

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@progress-default-color` | `defaultColor` | - |
| `@progress-remaining-color` | `remainingColor` | - |
| `@progress-info-text-color` | `colorText` | Global Token |
| `@progress-text-color` | `circleTextColor` | - |
| `@progress-radius` | `lineBorderRadius` | - |
| `@progress-steps-item-bg` | `remainingColor` | - |
| `@progress-text-font-size` | `fontSizeSM` | Global Token |
| `@progress-circle-text-font-size` | `circleTextFontSize` | - |

### Radio

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@radio-size` | `radioSize` | - |
| `@radio-top` | - | Deprecated |
| `@radio-border-width` | `lineWidth` | Global Token |
| `@radio-dot-size` | `dotSize` | - |
| `@radio-dot-color` | - | Deprecated |
| `@radio-dot-disabled-color` | `dotColorDisabled` | - |
| `@radio-solid-checked-color` | `buttonSolidCheckedColor` | - |
| `@radio-button-bg` | `buttonBg` | - |
| `@radio-button-checked-bg` | `buttonCheckedBg` | - |
| `@radio-button-color` | `buttonColor` | - |
| `@radio-button-hover-color` | `colorPrimaryHover` | Global Token |
| `@radio-button-active-color` | `colorPrimaryActive` | Global Token |
| `@radio-button-padding-horizontal` | `buttonPaddingInline` | - |
| `@radio-disabled-button-checked-bg` | `buttonCheckdBgDisabled` | - |
| `@radio-disabled-button-checked-color` | `buttonCheckdColorDisabled` | - |
| `@radio-wrapper-margin-right` | `wrapperMarginInlineEnd` | - |

### Rate

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@rate-star-color` | `starColor` | - |
| `@rate-star-bg` | `starBg` | - |
| `@rate-star-size` | `starSize` | - |
| `@rate-star-hover-scale` | `starHoverScale` | - |

### Result

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@result-icon-font-size` | `iconFontSize` | - |
| `@result-title-font-size` | `titleFontSize` | - |
| `@result-subtitle-font-size` | `subtitleFontSize` | - |
| `@result-extra-margin` | `extraMargin` | - |

### Segment

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@segmented-container-padding` | `padding` | - |
| `@segmented-label-color` | `itemColor` | - |
| `@segmented-hover-bg` | `itemHoverBg` | - |
| `@segmented-bg` | - | Could be customized with `className` or `style` |
| `@segmented-label-hover-color` | `itemHoverColor` | - |
| `@segmented-selected-bg` | `itemSelectedBg` | - |

<!-- ### Select -->

### Skeleton

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@skeleton-block-radius` | `blockRadius` | - |
| `@skeleton-title-height` | `titleHeight` | - |
| `@skeleton-color` | `gradientFromColor` | - |
| `@skeleton-to-color` | `gradientToColor` | - |
| `@skeleton-paragraph-margin-top` | `paragraphMarginTop` | - |
| `@skeleton-paragraph-li-height` | `paragraphLiHeight` | - |
| `@skeleton-paragraph-li-margin-top` | - | Deprecated for style change |

### Slider

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@slider-margin` | - | Could be customized with `className` or `style` |
| `@slider-rail-background-color` | `railBg` | - |
| `@slider-rail-background-color-hover` | `railHoverBg` | - |
| `@slider-track-background-color` | `trackBg` | - |
| `@slider-track-background-color-hover` | `trackHoverBg` | - |
| `@slider-handle-border-width` | `handleLineWidth` | - |
| `@slider-handle-background-color` | - | Deprecated |
| `@slider-handle-color` | `handleColor` | - |
| `@slider-handle-color-hover` | `handleActiveColor` | - |
| `@slider-handle-color-focus` | `handleActiveColor` | - |
| `@slider-handle-color-focus-shadow` | - Deprecated |
| `@slider-handle-color-tooltip-open` | `handleActiveColor` | - |
| `@slider-handle-size` | `handleSize` | - |
| `@slider-handle-margin-top` | - | Deprecated |
| `@slider-handle-margin-left` | - | Deprecated |
| `@slider-handle-shadow` | - | Deprecated |
| `@slider-dot-border-color` | `dotBorderColor` | - |
| `@slider-dot-border-color-active` | `dotActiveBorderColor` | - |
| `@slider-disabled-color` | `trackBgDisabled` | - |
| `@slider-disabled-background-color` | - | Deprecated |

### Statistic

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@statistic-title-font-size` | `titleFontSize` | - |
| `@statistic-content-font-size` | `contentFontSize` | - |
| `@statistic-font-family` | `fontFamily` | GlobalToken |

### Step

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@process-tail-color` | `colorSplit` | GlobalToken |
| `@steps-nav-arrow-color` | `navArrowColor` | - |
| `@steps-background` | `colorBgContainer` | - |
| `@steps-icon-size` | `iconSize` | - |
| `@steps-icon-custom-size` | `customIconSize` | - |
| `@steps-icon-custom-top` | `customIconTop` | - |
| `@steps-icon-custom-font-size` | `customIconFontSize` | - |
| `@steps-icon-top` | `iconTop` | - |
| `@steps-icon-font-size` | `iconFontSize` | - |
| `@steps-icon-margin` | - | Deprecated |
| `@steps-title-line-height` | `titleLineHeight` | - |
| `@steps-small-icon-size` | `iconSizeSM` | - |
| `@steps-small-icon-margin` | - | Deprecated |
| `@steps-dot-size` | `dotSize` | - |
| `@steps-dot-top` | - | Deprecated |
| `@steps-current-dot-size` | `dotCurrentSize` | - |
| `@steps-description-max-width` | `descriptionMaxWidth` | - |
| `@steps-nav-content-max-width` | `stepsNavContentMaxWidth` | - |
| `@steps-vertical-icon-width` | `iconSize` | - |
| `@steps-vertical-tail-width` | - | Deprecated |
| `@steps-vertical-tail-width-sm` | - | Deprecated |

<!-- ### Switch -->

### Table

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@table-bg` | `colorBgContainer` | Global Token |
| `@table-header-bg` | `headerBg` | - |
| `@table-header-color` | `headerColor` | - |
| `@table-header-sort-bg` | `headerSortActiveBg` | - |
| `@table-body-sort-bg` | `bodySortActiveBg` | - |
| `@table-row-hover-bg` | `rowHoverBg` | - |
| `@table-selected-row-color` | `colorText` | Global Token |
| `@table-selected-row-bg` | `rowSelectedBg` | - |
| `@table-body-selected-sort-bg` | - | Deprecated, same as `rowSelectedBg` |
| `@table-selected-row-hover-bg` | `rowSelectedHoverBg` | - |
| `@table-expanded-row-bg` | `rowExpandedBg` | - |
| `@table-padding-vertical` | `cellPaddingBlock` | - |
| `@table-padding-horizontal` | `cellPaddingInline` | - |
| `@table-padding-vertical-md` | `cellPaddingBlockMD` | - |
| `@table-padding-horizontal-md` | `cellPaddingInlineMD` | - |
| `@table-padding-vertical-sm` | `cellPaddingBlockSM` | - |
| `@table-padding-horizontal-sm` | `cellPaddingInlineSM` | - |
| `@table-border-color` | `borderColor` | - |
| `@table-border-radius-base` | `headerBorderRadius` | - |
| `@table-footer-bg` | `footerBg` | - |
| `@table-footer-color` | `footerColor` | - |
| `@table-header-bg-sm` | - | Deprecated, same as `headerBg` |
| `@table-font-size` | `cellFontSize` | - |
| `@table-font-size-md` | `cellFontSizeMD` | - |
| `@table-font-size-sm` | `cellFontSizeSM` | - |
| `@table-header-cell-split-color` | `headerSplitColor` | - |
| `@table-header-sort-active-bg` | `headerSortHoverBg` | Misused in v4, and used as hover bg actually |
| `@table-fixed-header-sort-active-bg` | `fixedHeaderSortActiveBg` | - |
| `@table-header-filter-active-bg` | `headerFilterHoverBg` | - |
| `@table-filter-btns-bg` | - | Deprecated, same as `filterDropdownBg` |
| `@table-filter-dropdown-bg` | `filterDropdownBg` | - |
| `@table-expand-icon-bg` | `expandIconBg` | - |
| `@table-selection-column-width` | `selectionColumnWidth` | - |
| `@table-sticky-scroll-bar-bg` | `stickyScrollBarBg` | - |
| `@table-sticky-scroll-bar-radius` | `stickyScrollBarBorderRadius` | - |

### Tabs

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@tabs-card-head-background` | `cardBg` | - |
| `@tabs-card-height` | `cardHeight` | - |
| `@tabs-card-active-color` | `itemSelectedColor` | - |
| `@tabs-card-horizontal-padding` | `cardPadding` | - |
| `@tabs-card-horizontal-padding-sm` | `cardPaddingSM` | - |
| `@tabs-card-horizontal-padding-lg` | `cardPaddingLG` | - |
| `@tabs-title-font-size` | `titleFontSize` | - |
| `@tabs-title-font-size-lg` | `titleFontSizeLG` | - |
| `@tabs-title-font-size-sm` | `titleFontSizeSM` | - |
| `@tabs-ink-bar-color` | `inkBarColor` | - |
| `@tabs-bar-margin` | `horizontalMargin` | - |
| `@tabs-horizontal-gutter` | `horizontalItemGutter` | - |
| `@tabs-horizontal-margin` | `horizontalItemMargin` | - |
| `@tabs-horizontal-margin-rtl` | `horizontalItemMarginRTL` | - |
| `@tabs-horizontal-padding` | `horizontalItemPadding` | - |
| `@tabs-horizontal-padding-lg` | `horizontalItemPaddingLG` | - |
| `@tabs-horizontal-padding-sm` | `horizontalItemPaddingSM` | - |
| `@tabs-vertical-padding` | `verticalItemPadding` | - |
| `@tabs-vertical-margin` | `verticalItemMargin` | - |
| `@tabs-scrolling-size` | - | Deprecated |
| `@tabs-highlight-color` | `itemSelectedColor` | - |
| `@tabs-hover-color` | `itemHoverColor` | - |
| `@tabs-active-color` | `itemActiveColor` | - |
| `@tabs-card-gutter` | `cardGutter` | - |
| `@tabs-card-tab-active-border-top` | - | Deprecated |

### Tag

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@tag-border-radius` | `borderRadiusSM` | Global Token |
| `@tag-default-bg` | `defaultBg` | - |
| `@tag-default-color` | `defaultColor` | - |
| `@tag-font-size` | `fontSizeSM` | Global Token |
| `@tag-line-height` | `lineHeightSM` | Global Token |

### Timeline

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@timeline-width` | `tailWidth` | `tailWidth`  is a number without units, `@timeline-width` with units |
| `@timeline-color` | `tailColor` | - |
| `@timeline-dot-border-width` | `dotBorderWidth` | - |
| `@timeline-dot-color` | - | Deprecated |
| `@timeline-dot-bg` | `dotBg` | - |
| `@timeline-item-padding-bottom` | `itemPaddingBottom` | - |

<!-- ### TimePicker -->

### Tooltip

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@tooltip-max-width` | - | Can be directly modified by `className` or `style` |
| `@tooltip-color` | `colorTextLightSolid` | Global Token |
| `@tooltip-bg` | `colorBgSpotlight` | Global Token |
| `@tooltip-arrow-width` | `sizePopupArrow` | Global Token |
| `@tooltip-distance` | `marginXXS` | Global Token |
| `@tooltip-arrow-color` | - | same as `@tooltip-bg`，Deprecated |
| `@tooltip-border-radius` | `borderRadius` | Global Token |

### Transfer

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@transfer-header-height` | `headerHeight` | - |
| `@transfer-item-height` | `itemHeight` | - |
| `@transfer-disabled-bg` | `colorBgContainerDisabled` | Global Token |
| `@transfer-list-height` | `listHeight` | - |
| `@transfer-item-hover-bg` | `controlItemBgHover` | Global Token |
| `@transfer-item-selected-hover-bg` | `controlItemBgActiveHover` | Global Token |
| `@transfer-item-padding-vertical` | `itemPaddingBlock` | - |
| `@transfer-list-search-icon-top` | - | Deprecated |

<!-- ### Tree -->

### Typography

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@typography-title-font-weight` | `fontWeightStrong` | Global Token |
| `@typography-title-margin-top` | `titleMarginTop` | - |
| `@typography-title-margin-bottom` | `titleMarginBottom` | - |

### Upload

<!-- prettier-ignore -->
| Less variables | Component Token | Note |
| --- | --- | --- |
| `@upload-actions-color` | `actionsColor` | - |
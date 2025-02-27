---
title: Navigation drawers
desc: "**MNavigationDrawer** is a component used to navigate applications. It is usually wrapped and used in the **MCard** element."
related:
  - /blazor/components/lists
  - /blazor/components/icons
  - /blazor/getting-started/wireframes
---

## Usage

Navigation navigation is mainly used to host links to pages in your application. It is common to pair drawers with
the [MList](/blazor/components/lists) component using the **Nav** property.

<masa-example file="Examples.components.navigation_drawers.Usage"></masa-example>

## Caveats

<app-alert type="error" content="If you are using **MNavigationDrawer** with **App** property enabled, you don't need to use `Absolute` prop as in examples."></app-alert>

<app-alert type="info" content="The `ExpandOnHover` prop does not alter the content area of **MMain**. To have content area respond to `ExpandOnHover`, bind `OnMiniVariantUpdate` to a data prop."></app-alert>

## Examples

### Props

#### Bottom drawer

Using the `Bottom` prop, we can reposition the drawer on the mobile device so that it emerges from the bottom of the screen. This is another style, which can only be activated when MobileBreakpoint is encountered.

<masa-example file="Examples.components.navigation_drawers.Bottom"></masa-example>

#### Expand on hover

Place the component in `MiniVariant` mode and expand when hovering. The content area of **MMain** that does not change.
The width can be controlled using the `MiniVariantWidth` property.

<masa-example file="Examples.components.navigation_drawers.ExpandOnHover"></masa-example>

#### Permanent and floating

By default, the navigation drawer has a 1px `Right` border to separate it from the content. In this example, we want to
separate the drawer from the left and let it float by itself. The `Floating` property can remove the right border (if
`Right` is used, the left border is removed).

<masa-example file="Examples.components.navigation_drawers.Floating"></masa-example>

#### Image

Apply a custom background to the drawer through the `Src` attribute. If you need to customize the properties
of **MImage**, you can use the `ImgContent`.

<masa-example file="Examples.components.navigation_drawers.Image"></masa-example>

#### Mini variant

When using the `MiniVariant` property, the drawer will shrink (56px by default) and hide all the contents in the **Mlist**
except the first element.

<masa-example file="Examples.components.navigation_drawers.Mini"></masa-example>

#### Right

The navigation drawer can also be placed on the right side of the application (or element). This is also useful for
creating side tables with auxiliary information that may not have any navigation links. When using **RTL**, you must clearly
define `Right` for the drawer.

<masa-example file="Examples.components.navigation_drawers.Right"></masa-example>

#### Temporary

use the `Temporary` prop The application that temporarily locates it starts, and this behavior is the default on the mobile device.

<masa-example file="Examples.components.navigation_drawers.Temporary"></masa-example>

### Misc

#### Colored drawer

The navigation drawer can be customized to fit the design of any application. Here we use the **AppendContent** to customize
the background color and additional content area.

<masa-example file="Examples.components.navigation_drawers.Color"></masa-example>

#### Constitute drawer

In this example, we defined a custom width to accommodate nested drawers. We use **MRow** to ensure that the drawer and
the list are horizontally adjacent to each other.

<masa-example file="Examples.components.navigation_drawers.Constitute"></masa-example>
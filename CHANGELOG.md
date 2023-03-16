## [2.1.0] 2023-03-16

- Migration to React 18
- Migration to Next.JS 13
- Update all dependencies
- Fix the installation issue

## [2.0.0] 2022-03-12

### Bug fixing

- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/20
- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/19
- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/17
- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/16
- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/13
- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/11
- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/10
- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/9
- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/8
- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/7
- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/6

### Major style changes

- Migration from Material-UI to MUI v5.
- Migration from JSS to `styled` api, emotion and `sx` prop.
- Product folders and files structured are updated: [README](https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/blob/main/README.md)
- New components are added
- New example blocks are added
- Components are Example Blocks are now totally customizable and reusable
- Product now uses the react context api for global configurations

### Deleted components

- Accordion
- Badge
- Card
- Clearfix
- CustomButtons
- CustomDropdown
- CustomInput
- CustomLinearProgress
- CustomTags
- CustomUpload
- FixedPlugin
- Footer
- Grid
- Heading
- Hooks
- InfoArea
- Intruction
- Navbars
- NavPills
- PageChange
- Pagination
- ReactTable
- Sidebar
- Snackbar
- Table
- TagsInput
- Tasks
- Timeline
- Typography
- Wizard
- WizardSteps

### Added components

- MDAlert
- MDAvatar
- MDBadge
- MDBadgeDot
- MDBox
- MDButton
- MDDatePicker
- MDDropzone
- MDEditor
- MDInput
- MDPagination
- MDProgress
- MDSnackbar
- MDSocialButton
- MDTypography
- Breadcrumbs
- Calendar
- Cards
  - BlogCards
    - SimpleBlogCard
  - BookingCard
  - ControllerCard
  - InfoCards
    - DefaultInfoCard
    - MiniInfoCard
    - ProfileInfoCard
  - MasterCard
  - PricingCards
    - DefaultPricingCard
  - ProjectCards
    - ComplexProjectCard
    - DefaultProjectCard
  - StatisticsCards
    - ComplexStatisticsCard
    - DefaultStatisticsCard
    - MiniStatisticsCard
- Charts
  - BarCharts
    - HorizontalBarChart
    - VerticalBarChart
    - ReportsBarChart
  - BubbleChart
  - DoughnutCharts
    - DefaultDoughnutChart
  - LineCharts
    - DefaultLineChart
    - GradientLineChart
    - ProgressLineChart
    - ReportsLineChart
  - MixedChart
  - PieChart
  - PolarChart
  - RadarChart
- Configurator
- Footer
- Items
  - DefaultItem
  - NotificationItem
- LayoutContainers
  - DashboardLayout
  - PageLayout
- Lists
  - CategoriesList
  - ProfilesList
- Navbars
  - DashboardNavbar
  - DefaultNavbar
- Sidenav
- Tables
  - DataTable
  - SalesTable
- Timeline
  - TimelineList
  - TimelineItem

### Deleted dependencies

```
@material-ui/core
@material-ui/icons
@zeit/next-css
@zeit/next-sass
chartist
classnames
history
match-sorter
moment
next-compose-plugins
next-images
node-sass
nouislider
path
perfect-scrollbar
react-big-calendar
react-bootstrap-sweetalert
react-chartist
react-datetime
react-jvectormap
react-swipeable-views
```

### Added dependencies

```
@asseinfo/react-kanban
@babel/preset-react
@mui/material
@mui/icons-material
@mui/styled-engine
@emotion/cache
@emotion/react
@emotion/server
@emotion/styled
@fullcalendar/common
@fullcalendar/daygrid
@fullcalendar/interaction
@fullcalendar/react
@fullcalendar/timegrid
@testing-library/jest-dom
@testing-library/react":
@testing-library/user-event
chart.js
chroma-js
dropzone
flatpickr
formik
html-react-parser
jsvectormap
next-transpile-modules
prop-types
react-chartjs-2
react-flatpickr
react-github-btn
react-html-parser
react-images-viewer
react-quill
regenerator-runtime
stylis
stylis-plugin-rtl
uuid
web-vitals
yup
```

### Updated dependencies

```
next            10.0.5   →   12.1.0
react           17.0.1   →   17.0.2
react-dom       17.0.1   →   17.0.2
react-table     7.6.3    →   7.7.0
```

### Warning

## [1.1.0] 2021-02-01

### Bug fixing

- changed the class component from `pages/_error.js` to functional one for hooks support
- changed the class component from `pages/404.js` to functional one for hooks support
- changed the class component from `pages/index.js` to functional one for hooks support
- changed the class component from `components/WizardSteps/step1.js` to functional one for hooks support
- changed the class component from `components/WizardSteps/step2.js` to functional one for hooks support
- changed the class component from `components/WizardSteps/step3.js` to functional one for hooks support
- changed the class component from `components/Sidebar/Sidebar.js` to functional one for hooks support
- At the moment `pages/_app.js`, `pages/_document.js` and `components/Wizard/Wizard.js` could not be converted to functional components, please check the bellow warnings for more information
- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/4
- https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/2 (check solution here: https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/2#issuecomment-769083707)

### Major style changes

- Moved all usages of `makeStyles` function, to inside of the functional components, rather than outside of them (please check more here: https://github.com/creativetimofficial/ct-nextjs-material-dashboard-pro/issues/2#issuecomment-769083707)
- `assets/jss/nextjs-material-dashboard-pro/views/lockScreenPageStyle.js` (since solving #2, we needed to add `!important` rule on some styles)
- Inside `pages/admin/sweet-alert.js` removed the usage of `makeStyles` and replaced it with `withStyles` (since the solution for #2 was affecting the styles on this page)
- `assets/jss/nextjs-material-dashboard-pro/components/wizardStyle.js` (since the solution for #2 was affecting the styles on this component)
- `assets/jss/nextjs-material-dashboard-pro/views/extendedTablesStyle.js` (since solving #2, we needed to add `!important` rule on some styles)
- `assets/jss/nextjs-material-dashboard-pro/buttonGroupStyle.js` (since solving #2, we needed to add `!important` rule on some styles)

### Deleted components

### Added components

- `components/TagsInput/TagsInput.js` instead of `react-tagsinput` - NOTE, `components/TagsInput/TagsInput.js` is the exact component as `react-tagsinput`, but it uses React Hooks instead.

### Deleted dependencies

- @types/googlemaps
- @types/markerclustererplus
- react-google-maps (we'll use simple Google Maps API with Vanilla JS instead)
- react-tagsinput (We've added a new component inside `components/TagsInput/TagsInput.js` which is the exact same as `react-tagsinput` but it uses React 17)

### Added dependencies

### Updated dependencies

```
@material-ui/core       4.11.0   →   4.11.3
@material-ui/icons       4.9.1   →   4.11.2
match-sorter             4.2.0   →    6.1.0
moment                  2.27.0   →   2.29.1
next                     9.5.2   →   10.0.5
next-compose-plugins     2.2.0   →    2.2.1
next-images              1.3.1   →    1.7.0
nouislider              14.6.1   →   14.6.3
react                  16.13.1   →   17.0.1
react-big-calendar      0.26.0   →   0.30.0
react-datetime          2.16.3   →    3.0.4
react-dom              16.13.1   →   17.0.1
react-table              7.5.0   →    7.6.3
webpack                 4.44.1   →   5.17.0
typescript               3.9.7   →    4.1.3
```

### Warning

**At the moment, the `pages/_app.js` and `pages/_document.js` could not be converted to functional components - for HOOK support, since they still need some of the class comments life-cycle methods. Please check this here: https://nextjs.org/docs/advanced-features/custom-document.**
**Also, the `components/Wizard/Wizard.js` was not changed to hooks since it needs some of the class lifecycle methods.**
**The TypeScript dependencies are installed only to stop console warnings on install. They are not actually used in our product. So the product is not based on TypeScript!**
_The following warnings will appear when running the installation command, but they do not affect the UI or the functionality of the product (they will be solved in our next update):_

```
npm WARN react-big-calendar@0.30.0 requires a peer of react@^16.6.1 but none is installed. You must install peer dependencies yourself.
npm WARN react-big-calendar@0.30.0 requires a peer of react-dom@^16.6.1 but none is installed. You must install peer dependencies yourself.
npm WARN react-chartist@0.14.3 requires a peer of react@^0.14.9 || ^15.0.0 || ^16.0.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-datetime@3.0.4 requires a peer of react@^16.5.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-swipeable-views@0.13.9 requires a peer of react@^15.3.0 || ^16.0.0 but none is installed. You must install peer dependencies yourself.
npm WARN css-loader@1.0.0 requires a peer of webpack@^4.0.0 but none is installed. You must install peer dependencies yourself.
npm WARN mini-css-extract-plugin@0.4.3 requires a peer of webpack@^4.4.0 but none is installed. You must install peer dependencies yourself.
npm WARN terser-webpack-plugin@1.4.5 requires a peer of webpack@^4.0.0 but none is installed. You must install peer dependencies yourself.
npm WARN react-event-listener@0.6.6 requires a peer of react@^16.3.0 but none is installed. You must install peer dependencies yourself.
```

_If they will persist in our 2.*.* version, we will drop their usages and replace them with other plugins._
_In development mode, some of the above plugins will throw a warning because they still use React v16 syntax. If the error will persist in our 2.*.* version, we will drop their usage and replace them with other plugins._

## [1.0.0] 2020-08-19

### Original Release

- Started project with NextJS
- Added design from Material Dashboard PRO React by Creative Tim

### Warning

_Warnings might appear while doing an npm install - they do not affect the UI or the functionality of the product, and they appear because of NodeJS and not from the product itself._
_While in development some of the plugins that were used for this product will throw some warnings - note, this only happens in development, the UI or the functionality of the product is not affected, also, if the issues will persist in React 17, we'll drop usage of those plugins, and replace them with other ones._

- Added new options, axis.softMin and axis.softMax. Closes #5824.
- Added Legend keyboard navigation to the accessibility module.
- Added animation on hovering point markers.
- Added offline PDF export support.
## Bug fixes 
- Refactored tooltip delay the generation of the empty label container. This prevents the empty label from being present in exported SVG.
- Fixed #1880, individual column ``borderColor``.
- Fixed #4951, issue with placing tick marks on round times when using ``getTimezoneOffset``.
- Fixed #5427, JS error on async destroy when triggered from custom exporting menu.
- Fixed #5483 without breaking #5823.
- Fixed #5538, pie series was not redrawn after modifying title and other elements.
- Fixed #5553, disabled ``trackByArea`` did not hide tooltip, when moving mouse out of the area shape.
- Fixed #5736, zooming in multiple X axes with crosshairs and snap false caused JS error.
- Fixed #5745, a regression causing ``chart.style`` not to apply to the container.
- Fixed #5750, null points on categorized axis caused blank chart when drilldown module was present.
- Fixed #5757, empty chart throws error with accessibility module.
- Fixed #5764, drilldown not working with Highstock.
- Fixed #5765, a regression causing 3D pie slices not to update on show/hide when animation was set.
- Fixed #5766, halo was not rendered for shared tooltip when density of points was high.
- Fixed #5768, regression since v4.2.7 causing setData with xAxis.type = category to break categories.
- Fixed #5770, regression causing individual box plot fill not to apply.
- Fixed #5773, a regression causing axis events not to be called after axis update.
- Fixed #5777, selected class name remained after unselecting a point by selecting another.
- Fixed #5779, zoom-out button not working on first touch on touch devices.
- Fixed #5787, a regression causing the ``chart.reflow`` option to never take effect.
- Fixed #5790, zoom button appeared on swiping already zoomed-out line chart.
- Fixed #5794, header on ``tooltip.split`` was cut off near the ends of the axis.
- Fixed #5801, artefacts when updating series with tooltip.split.
- Fixed #5817, a regression causing point-specific marker radius not to be applied. Refactored point sizing logic for initial render, updates and states.
- Fixed #5818, render halo in a series group, not under all of the groups.
- Fixed #5819, crosshair width can now be set on category axes also.
- Fixed #5822, a regression causing drilldown to fail the second time when ``allowPointDrilldown`` was false.
- Fixed #5832, shared tooltip failed with points of the same X value but different pointPlacement.
- Fixed #5833, split tooltip tried to remove series tooltip again after destruction.
- Fixed #5837, could not style null points with CSS.
- Fixed #5839, errors on touch-dragging on mobile devices after dynamically adding a series with visible false.
- Fixed #5842, image marker symbols were misplaced and missing from exported charts.
- Fixed #5850, hideLoading didn't work right after calling showLoading in styled mode.
- Fixed #5855, split tooltip was not destroyed properly.
- Fixed #5862, wrong hover point, when tooltip was shared.
- Fixed #5866, treemap ``point.isNull`` was always true.
- Fixed duplicate setting of halo path since HC5. Added animation to hiding halo.
- Fixed eternal loop when setting a new ``chart.height`` in a responsive rule.
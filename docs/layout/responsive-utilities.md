---
layout: page
title: Responsive utilities
---

For faster mobile-friendly development, use these utility classes for showing and hiding content by device via media query. Also included are utility classes for toggling content when printed.

Try to use these on a limited basis and avoid creating entirely different versions of the same site. Instead, use them to complement each device's presentation.

##  Available classes

Use a single or combination of the available classes for toggling content across viewport breakpoints.

<div class="table-responsive">
  <table class="table table-bordered table-striped responsive-utilities">
    <thead>
      <tr>
        <th></th>
        <th>
          Extra small devices
          <small>Phones (&lt;768px)</small>
        </th>
        <th>
          Small devices
          <small>Tablets (&ge;768px)</small>
        </th>
        <th>
          Medium devices
          <small>Desktops (&ge;992px)</small>
        </th>
        <th>
          Large devices
          <small>Desktops (&ge;1200px)</small>
        </th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th scope="rowspan"><code>.visible-xs-*</code></th>
        <td class="is-visible">Visible</td>
        <td class="is-hidden">Hidden</td>
        <td class="is-hidden">Hidden</td>
        <td class="is-hidden">Hidden</td>
      </tr>
      <tr>
        <th scope="rowspan"><code>.visible-sm-*</code></th>
        <td class="is-hidden">Hidden</td>
        <td class="is-visible">Visible</td>
        <td class="is-hidden">Hidden</td>
        <td class="is-hidden">Hidden</td>
      </tr>
      <tr>
        <th scope="rowspan"><code>.visible-md-*</code></th>
        <td class="is-hidden">Hidden</td>
        <td class="is-hidden">Hidden</td>
        <td class="is-visible">Visible</td>
        <td class="is-hidden">Hidden</td>
      </tr>
      <tr>
        <th scope="rowspan"><code>.visible-lg-*</code></th>
        <td class="is-hidden">Hidden</td>
        <td class="is-hidden">Hidden</td>
        <td class="is-hidden">Hidden</td>
        <td class="is-visible">Visible</td>
      </tr>
    </tbody>
    <tbody>
      <tr>
        <th scope="rowspan"><code>.hidden-xs</code></th>
        <td class="is-hidden">Hidden</td>
        <td class="is-visible">Visible</td>
        <td class="is-visible">Visible</td>
        <td class="is-visible">Visible</td>
      </tr>
      <tr>
        <th scope="rowspan"><code>.hidden-sm</code></th>
        <td class="is-visible">Visible</td>
        <td class="is-hidden">Hidden</td>
        <td class="is-visible">Visible</td>
        <td class="is-visible">Visible</td>
      </tr>
      <tr>
        <th scope="rowspan"><code>.hidden-md</code></th>
        <td class="is-visible">Visible</td>
        <td class="is-visible">Visible</td>
        <td class="is-hidden">Hidden</td>
        <td class="is-visible">Visible</td>
      </tr>
      <tr>
        <th scope="rowspan"><code>.hidden-lg</code></th>
        <td class="is-visible">Visible</td>
        <td class="is-visible">Visible</td>
        <td class="is-visible">Visible</td>
        <td class="is-hidden">Hidden</td>
      </tr>
    </tbody>
  </table>
</div>

As of v3.2.0, the `.visible-*-*` classes for each breakpoint come in three variations, one for each CSS `display` property value listed below.

<div class="table-responsive">
  <table class="table table-bordered table-striped">
    <thead>
      <tr>
        <th>Group of classes</th>
        <th>CSS <code>display</code></th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><code>.visible-*-block</code></td>
        <td><code>display: block;</code></td>
      </tr>
      <tr>
        <td><code>.visible-*-inline</code></td>
        <td><code>display: inline;</code></td>
      </tr>
      <tr>
        <td><code>.visible-*-inline-block</code></td>
        <td><code>display: inline-block;</code></td>
      </tr>
    </tbody>
  </table>
</div>
<p>So, for extra small (<code>xs</code>) screens for example, the available <code>.visible-*-*</code> classes are: <code>.visible-xs-block</code>, <code>.visible-xs-inline</code>, and <code>.visible-xs-inline-block</code>.</p>

<h2 id="responsive-utilities-print">Print classes</h2>
<p>Similar to the regular responsive classes, use these for toggling content for print.</p>
<div class="table-responsive">
  <table class="table table-bordered table-striped responsive-utilities">
    <thead>
      <tr>
        <th>Classes</th>
        <th>Browser</th>
        <th>Print</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th>
          <code>.visible-print-block</code><br>
          <code>.visible-print-inline</code><br>
          <code>.visible-print-inline-block</code>
        </th>
        <td class="is-hidden">Hidden</td>
        <td class="is-visible">Visible</td>
      </tr>
      <tr>
        <th><code>.hidden-print</code></th>
        <td class="is-visible">Visible</td>
        <td class="is-hidden">Hidden</td>
      </tr>
    </tbody>
  </table>
</div>

## Test cases

Resize your browser or load on different devices to test the responsive utility classes.

### Visible on...

Green checkmarks indicate the element **is visible** in your current viewport.

<div class="row responsive-utilities-test visible-on">
  <div class="col-xs-6 col-sm-3">
    <span class="hidden-xs">Extra small</span>
    <span class="visible-xs-block">&#10004; Visible on x-small</span>
  </div>
  <div class="col-xs-6 col-sm-3">
    <span class="hidden-sm">Small</span>
    <span class="visible-sm-block">&#10004; Visible on small</span>
  </div>
  <div class="clearfix visible-xs-block"></div>
  <div class="col-xs-6 col-sm-3">
    <span class="hidden-md">Medium</span>
    <span class="visible-md-block">&#10004; Visible on medium</span>
  </div>
  <div class="col-xs-6 col-sm-3">
    <span class="hidden-lg">Large</span>
    <span class="visible-lg-block">&#10004; Visible on large</span>
  </div>
</div>
<div class="row responsive-utilities-test visible-on">
  <div class="col-xs-6">
    <span class="hidden-xs hidden-sm">Extra small and small</span>
    <span class="visible-xs-block visible-sm-block">&#10004; Visible on x-small and small</span>
  </div>
  <div class="col-xs-6">
    <span class="hidden-md hidden-lg">Medium and large</span>
    <span class="visible-md-block visible-lg-block">&#10004; Visible on medium and large</span>
  </div>
  <div class="clearfix visible-xs-block"></div>
  <div class="col-xs-6">
    <span class="hidden-xs hidden-md">Extra small and medium</span>
    <span class="visible-xs-block visible-md-block">&#10004; Visible on x-small and medium</span>
  </div>
  <div class="col-xs-6">
    <span class="hidden-sm hidden-lg">Small and large</span>
    <span class="visible-sm-block visible-lg-block">&#10004; Visible on small and large</span>
  </div>
  <div class="clearfix visible-xs-block"></div>
  <div class="col-xs-6">
    <span class="hidden-xs hidden-lg">Extra small and large</span>
    <span class="visible-xs-block visible-lg-block">&#10004; Visible on x-small and large</span>
  </div>
  <div class="col-xs-6">
    <span class="hidden-sm hidden-md">Small and medium</span>
    <span class="visible-sm-block visible-md-block">&#10004; Visible on small and medium</span>
  </div>
</div>

### Hidden on...

Here, green checkmarks also indicate the element **is hidden** in your current viewport.

<div class="row responsive-utilities-test hidden-on">
  <div class="col-xs-6 col-sm-3">
    <span class="hidden-xs">Extra small</span>
    <span class="visible-xs-block">&#10004; Hidden on x-small</span>
  </div>
  <div class="col-xs-6 col-sm-3">
    <span class="hidden-sm">Small</span>
    <span class="visible-sm-block">&#10004; Hidden on small</span>
  </div>
  <div class="clearfix visible-xs-block"></div>
  <div class="col-xs-6 col-sm-3">
    <span class="hidden-md">Medium</span>
    <span class="visible-md-block">&#10004; Hidden on medium</span>
  </div>
  <div class="col-xs-6 col-sm-3">
    <span class="hidden-lg">Large</span>
    <span class="visible-lg-block">&#10004; Hidden on large</span>
  </div>
</div>
<div class="row responsive-utilities-test hidden-on">
  <div class="col-xs-6">
    <span class="hidden-xs hidden-sm">Extra small and small</span>
    <span class="visible-xs-block visible-sm-block">&#10004; Hidden on x-small and small</span>
  </div>
  <div class="col-xs-6">
    <span class="hidden-md hidden-lg">Medium and large</span>
    <span class="visible-md-block visible-lg-block">&#10004; Hidden on medium and large</span>
  </div>
  <div class="clearfix visible-xs-block"></div>
  <div class="col-xs-6">
    <span class="hidden-xs hidden-md">Extra small and medium</span>
    <span class="visible-xs-block visible-md-block">&#10004; Hidden on x-small and medium</span>
  </div>
  <div class="col-xs-6">
    <span class="hidden-sm hidden-lg">Small and large</span>
    <span class="visible-sm-block visible-lg-block">&#10004; Hidden on small and large</span>
  </div>
  <div class="clearfix visible-xs-block"></div>
  <div class="col-xs-6">
    <span class="hidden-xs hidden-lg">Extra small and large</span>
    <span class="visible-xs-block visible-lg-block">&#10004; Hidden on x-small and large</span>
  </div>
  <div class="col-xs-6">
    <span class="hidden-sm hidden-md">Small and medium</span>
    <span class="visible-sm-block visible-md-block">&#10004; Hidden on small and medium</span>
  </div>
</div>
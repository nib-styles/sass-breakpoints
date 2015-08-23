# @nib-styles/sass-breakpoints

SASS mixins for named breakpoints.

## Installation

    npm install --save @nib-styles/sass-breakpoints

## Usage

    sass-composer example/example.scss -o compiled.css

SCSS: `example/example.scss`

    @import "@nib-styles/sass-breakpoints";
    
    @include breakpoint('sm') {           //from `sm` (>=0px)
      body { background-color: red; }
    }
    
    @include breakpoint('lg') {           //from `lg` (>=800px)
      body { background-color: green; }
    }

CSS: `compiled.css`
    
    @media (min-width: 30em) {
      body {
        background-color: red; } }
    
    @media (min-width: 50em) {
      body {
        background-color: green; } }

See [sass-breakpoints](https://www.npmjs.com/package/sass-breakpoints) for a full list of the available mixins.

## Breakpoints

<table width="25%">
  <tr>
    <th width="25%">Name</th>
    <th>Resolution</th>
  </tr>
  <tr>
    <td>xs</td>
    <td>0px</td>
  </tr>
  <tr>
    <td>sm</td>
    <td>480px</td>
  </tr>
  <tr>
    <td>md</td>
    <td>640px</td>
  </tr>
  <tr>
    <td>lg</td>
    <td>800px</td>
  </tr>
  <tr>
    <td>xl</td>
    <td>960px</td>
  </tr>
</table>

# Design Piece

For a design piece I’m proud of, I chose to display a Wolfson donation form. I don't design movie posters and billboards but I do take content and make is visually appealing and presentable. I chose to share this because a lot of the ‘design’ work I do is about making hierarchical decisions. Often times I find myself needing to present a lot of information on one page and the challenge is usually to present the content in a way that doesn’t overwhelm the user. Below you’ll see a small screen view of the form that uses a simple JavaScript toggle to hide information until the user selects a checkbox indicating they need the extra form elements. Then they are displayed.

![wch-donate.gif](https://s1.gifyu.com/images/wch-donate.gif)


![wch-donate-toggle.gif](https://s1.gifyu.com/images/wch-donate-toggle.gif)


# Development Piece

For my development piece with logic I thought I would pick one of the text utility patterns used to create my portfolio. This code is a handlebars.js file that takes data (in this instance brand colors) from a colors.yaml file and prints them on a page. I didn’t choose this piece because of complexity, in fact the exact opposite. To me it’s a great example of how designs can be presented quickly to a client using minimal markup and logic. I thought it would be relevant to the UI Designer position that practices live wireframing. 

``` hbs
{{#each (data "colors")}}
  {{#each this}}
    {{#if textClass}}
      <p class="{{textClass}}">
        {{textClass}}
      </p>
    {{/if}}
  {{/each}}
{{/each}}
```

```yml
brand:
  - color: "#C5C5BD"
    property: "--color-greenLight"
    bgClass: "u-bgGreenLight"
    borderClass: "u-borderColorGreenLight"
    textClass: "u-textGreenLight"
  - color: "#6C8A82"
    property: "--color-green"
    bgClass: "u-bgGreen"
    borderClass: "u-borderColorGreen"
    textClass: "u-textGreen"
  - color: "#5C635B"
    property: "--color-greenDark"
    bgClass: "u-bgGreenDark"
    borderClass: "u-borderColorGreenDark"
    textClass: "u-textGreenDark"
  - color: "#E4D5BE"
    property: "--color-beige"
    bgClass: "u-bgBeige"
    borderClass: "u-borderColorBeige"
    textClass: "u-textBeige"
  - color: "#DBD3D0"
    property: "--color-peach"
    bgClass: "u-bgPeach"
    borderClass: "u-borderColorPeach"
    textClass: "u-textPeach"
```

# Changelog
_These releases contain markup changes and potentially breaking changes. <br>
A :warning: icon indicates where we've made a change that might be a breaking change for your project. <br>
A :pushpin: icon indicates a markup change that is not a breaking change._

## 1.1.0
January 1, 2022
<!--
Include:
- Benefit statement
- Brief description of the update
- Use consistent, active verbs like "Fixed", "Added", "Improved" to indicate the type of change
- Present items in order of category: Bug fixes, enhancements, new features, deprecations
- Make content scannable by using nested list items 
Ex: ** **
-->

### General
- Fixed the baseline alignment in the unstyled button variant. (#4812)
- Added a LinkedIn icon and included it in our default icon sprite as `linkedin`. (#4812)
- Added type="button" to all non-form buttons to prevent default submit behaviors. (#4812)
    - This allowed us to remove preventDefault() from the relevant component JS.
    - :warning: This is a potentially breaking change. Teams should update all non-form buttons to include type="button" in their markup. <button> elements that do not receive a defined type attribute will inherit type="submit" behaviors by default. This can cause unintended and undesired behavior in our buttons. Resource: Details on button types (Mozilla) (#4695)
- Updated markup in the usa-password package to use a <button> element instead of an anchor element. (#4847)
    - This markup is more semantically appropriate for the related on-page user interaction.
    - :pushpin: This is not a breaking change. The old markup is still supported, but teams should consider updating to the new markup for improved semantics. 
        #### Old
        ```
        <p class="usa-form__note">
          <a href="#" class="usa-show-multipassword" aria-controls="password confirmPassword"
            data-hide-text="Hide my typing">Show my typing</a>
        </p>
        ```

       #### New
       ```
       <button type="button" 
          class="usa-show-password usa-button usa-button--unstyled" 
          aria-controls="password confirmPassword"
          data-hide-text="Hide my typing">Show my typing</button>
        ```

### Performance
- Optimized the hero image.(#4812)
    - We replaced our default hero image (644 KB PNG) with an optimized image (147 KB JPG), saving 477 KB. We've also provided a next-generation image format version of the image (105 KB WEBP) as an example.
    - :warning: This is a potentially breaking change. This changes the value of $theme-hero-image. If your project uses this default hero image, you'll need to make sure to move the new asset (hero.jpg) to your project images directory.

### Accessibility
- Added styles for `aria-disabled` to match `disabled`. (#4783)
    - Now disabled styling is applied whether you use `disabled` (disabled and hidden from screen readers) or `aria-disabled` (disabled and visible to screen readers). 

### Dependency updates
_No dependency updates_
0 vulnerabilities in regular dependencies (dependencies for USWDS projects installed with npm install uswds)

Internal only: 3 moderate, 32 high vulnerabilities in devDependencies (development dependencies)

Release TGZ SHA-256 hash: 727a1883badb336f67f6f355e8fdf7ace9af871ca8af7dbb231b2e3cc7649a9b

## 1.0.0
January 1, 2022

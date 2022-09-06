# Changelog

_These releases contain markup changes and potentially breaking changes.
A warning icon (:warning:) indicates where we've made an update that might be a breaking change for your project._

## v1.1.0

January 2, 2022

### General
- Added a LinkedIn icon and included it in our default icon sprite as `linkedin`. (https://github.com/uswds/uswds/pull/4872)

### Accessibility

- Added styles for `aria-disabled` to match `disabled`. (https://github.com/uswds/uswds/pull/4812)
    - Now disabled styling is applied whether you use `disabled` (disabled and hidden from screen readers) or `aria-disabled` (disabled and visible to screen readers).
- Updated markup in the usa-password package to use a `<button>` element instead of an anchor element. (https://github.com/uswds/uswds/pull/4847)
    - This markup is more semantically appropriate for the related on-page user interaction.
    - This is not a breaking change. The old markup is still supported, but teams should consider updating to the new markup for improved semantics.

        **Old**
        ```
        <p class="usa-form__note">
          <a href="#" class="usa-show-multipassword" aria-controls="password confirmPassword"
            data-hide-text="Hide my typing">Show my typing</a>
        </p>
        ```
       **New**
       ```
       <button type="button"
          class="usa-show-password usa-button usa-button--unstyled"
          aria-controls="password confirmPassword"
          data-hide-text="Hide my typing">Show my typing</button>
        ```

### Performance

- Optimized the hero image. (https://github.com/uswds/uswds/pull/4812)
    - We replaced our default hero image (644 KB PNG) with an optimized image (147 KB JPG), saving 477 KB. We've also provided a next-generation image format version of the image (105 KB WEBP) as an example.
    - :warning: This is a potentially breaking change. This changes the value of $theme-hero-image. If your project uses this default hero image, you'll need to make sure to move the new asset (hero.jpg) to your project images directory.

### Visual

- Fixed the baseline alignment in the unstyled button variant. (https://github.com/uswds/uswds/pull/4812)

## v1.0.0

January 1, 2022

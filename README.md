# angularMotorola

### feature-1

- Introduce the [$route] service which allows binding URLs for deep-linking with
  views:
  - Create `PhoneCatCtrl` which governs the entire app and contains $route configuration.
  - Install `angular-route` using bower and load the `ngRoute` module.
    (Be sure to run npm install again.)
  - Copy route parameters to root scope `params` property for access in sub controllers.
  - Replace the contents of `index.html` with the `ngView` directive, which will display the partial
    template of the current route.

- Create phone list route:
  - Map `/phones` route to `PhoneListCtrl` and `partials/phones-list.html`.
  - Preserve existing `PhoneListCtrl` controller.
  - Move existing html from `index.html` to `partials/phone-list.html`.
- Create phone details route:
  - Map `/phones/<phone-id>` route to `PhoneDetailCtrl` and `partials/phones-detail.html`.
  - Create empty placeholder `PhoneDetailsCtrl` controller.

### feature-2


- Implement `PhoneDetailCtrl` controller to fetch the details for a specific phone from a JSON file
  using `$http` service.
- Update the template for the phone detailed view.
- Add CSS to make the phone details page look "pretty".
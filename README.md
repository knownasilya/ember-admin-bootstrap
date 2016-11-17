# Ember Admin Bootstrap

Bootstrap theme for Ember Admin.

## Usage

Setup this and the theme manager addon:

```sh
ember install ember-admin-bootstrap
ember install ember-admin-theme-manager
```

Then add the following to your app's `application` template:

```hbs
{{#admin-theme-manager theme='bootstrap' adminConfig=adminConfig as |theme|}}
  {{#if (eq theme 'bootstrap')}}
    {{mount 'ember-admin-bootstrap'}}
  {{/if}}
{{/admin-theme-manager}}
```

Note: we use `ember-truth-helpers` addon for the `(eq ` part.

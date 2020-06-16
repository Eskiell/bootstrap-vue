# VUE 3

## Todo Items:

- Modal manager needs to be reworked to no longer be a component.
- The event system has changed, so `this.$once` and `listendOnRoot` calls need to be reworked.
- The render functions need to be updated as it appears that `h` is no longer supplied and needs to
  be imported from `vue`.
- The toast system needs to be fully tested as it switched from `vue-portal` to Vue 3's `teleport`.

## Posibilities:

- `defineComponent` is really only needed when working with TS. This could either be removed, or the
  project can be switched to TS.
- The components can be updated to use the new composition API instead of the options api.

## Roadblocks:

- Nuxt does not have an updated release that is compatable with Vue3. The current release still
  requires `vue-template-compiler` which is incompatable with Vue 3. This is causing jest to error
  with version mismatch between Vue and `vue-template-compiler`
